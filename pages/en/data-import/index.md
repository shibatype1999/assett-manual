# Data Import (Screenshots and CSV)
<!-- position: 10 -->
<!-- description: How to import assets and balances in bulk from screenshots of banking or brokerage apps, or from CSV files from Excel, Numbers, and other apps. -->

You can bring in the assets and balances you managed in other apps or spreadsheets all at once.
Choose how to import under **Settings** → **Data import**.

| Method | Description |
| --- | --- |
| From screenshots | Reads asset names and amounts from screenshots of balance screens in banking, brokerage, or points apps. |
| From a CSV file | Imports a CSV file exported from Excel, Numbers, a budgeting app, and so on. You can move past records too. |

Everything is read on your device. Images and file contents are never sent anywhere.

![Data import](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/data-import.png)

> **Point**
> Before importing, the app automatically makes a local backup of your current data. Right after an import, you can tap **Undo import** on the completion screen to go back to how things were before.

## Importing from screenshots

### 1. Take screenshots

1. In your banking, brokerage, or points app, open a balance screen that lists asset names and amounts.
2. Press the side button and the volume up button at the same time to take a screenshot. If the screen is long, take several screenshots.

**Tips for better reading**

- Turn off hidden balances (***).
- Choose screens where the name and amount are on the same line.
- Close banners and pop-ups before taking the shot.
- If an "as of" date is shown, records use that date.

**How to take screenshots** on the **Data import** screen shows examples of screens that can and can't be read.

### 2. Read them

1. Tap **Settings** → **Data import** → **From screenshots**.
2. The first time, you are asked for permission to access your photos. Allow it.
3. Select the screenshots you took.
4. When reading is finished, the **Review import** screen opens.

### 3. Review and save

The **Review import** screen works the same way as for CSV files (→ "Reviewing and saving the import" below).

### Deleting the imported screenshots

After saving, the imported screenshots are **automatically deleted from Photos**.

- iOS asks you to confirm the deletion.
- Deleted screenshots can be recovered from **Recently Deleted** in the Photos app for 30 days.
- If you allowed access to selected photos only, for example, the screenshots may not be deleted. In that case, allow full Photos access, or delete them in the Photos app.

## Importing from a CSV file

### 1. Prepare a CSV file

Use the first row for headings. Either of the following layouts can be imported.

**A. Rows (recommended)** – One record per row. Date, asset, and amount are required; currency, subcategory, and memo can be omitted.

| Date | Asset | Amount | Currency | Sub-category | Memo |
| --- | --- | --- | --- | --- | --- |
| 2026/09/30 | Bank A | 12,500 | USD | Month-end | |
| 2026/09/30 | Broker B | 3,500 | USD | | |
| 2026/09/30 | Mortgage | -180,000 | | | |

**B. Columns** – One date per row, with a column for each asset from the second column on. This is the same shape as a typical budget trend sheet.

| Date | Bank A | Broker B | Mortgage |
| --- | --- | --- | --- |
| 2026/08/31 | 12,000 | 3,400 | -181,000 |
| 2026/09/30 | 12,500 | 3,500 | -180,000 |

**Rules**

- Date: 2026/09/30, 2026-09-30, 09/30/2026, etc.
- Amount: commas and currency symbols are fine. Debts are negative (-).
- Currency: a code such as USD or JPY. Blank means the asset's currency.
- Asset: names not in the app can be created as new assets.
- Encoding: UTF-8 or Shift_JIS.
- Files can be up to 5 MB.

Tap **Export a CSV template** on the **Data import** screen to export a template with headings. If you already have assets, **Export template (with your assets)** creates a template that includes your current asset names.

**Saving from Excel or Numbers**

- Excel: File → Save As → "CSV UTF-8"
- Numbers: File → Export To → CSV

Then send the file to your iPhone with the Files app or by email.

### 2. Assign the columns

1. Tap **Settings** → **Data import** → **From a CSV file** and choose the CSV file.
2. On the CSV screen, check the layout (**Rows** or **Columns**). It is detected automatically; switch it if it's wrong.
3. Under **Columns**, check whether each column is **Date**, **Asset**, **Amount**, **Currency**, **Sub-category**, **Memo**, or **Don't use**. Columns are assigned automatically from the headings.
4. Check the results in **Preview (first 3)** and tap **Next (review …)**.

## Reviewing and saving the import

The **Review import** screen shows, for each name that was read, where it will be saved and the amount (or number of records).

![Review import](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/data-import-review.png)

1. Check where each name will be saved.
   - **Existing** – Records are added to an asset already in the app.
   - **New** – A new asset is created. Its icon, currency, and category are suggested from the name. Assets whose records are all negative (such as loans) are created as liabilities.
   - Tap a row to choose again: an existing asset, **Create new asset "…"**, or **Don't import**.
2. Rows whose amount couldn't be read are marked **Enter**. If you don't enter an amount, the row isn't saved.
3. For screenshots, check the date for the records. For CSV records without a date, the date chosen under **Date for records without one** is used.
4. Under **If a record exists on the same date**, choose **Overwrite** or **Skip**.
5. Tap **Save …**.

When saving is finished, the **Import complete** screen appears.

- The app remembers how names were matched to assets, and matches them automatically next time.
- Tap **Import more** to import more screenshots or files.
- Tap **Undo import** to go back to how things were before the import.

> **Caution**
> Asset names and amounts that are read may contain errors. Always check them before saving.
