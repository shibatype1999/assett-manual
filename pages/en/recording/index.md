# Recording Balances
<!-- position: 3 -->
<!-- description: The four ways to record balances on the Input tab (Quick entry, Batch, By asset, and Calendar), editing and deleting records, and reading the record list. -->

You record balances on the **Input** tab (screen title **Asset input**). Use the tabs at the top of the screen to switch between four ways of recording. The tab you used last is selected the next time you open it.

| Tab | Best for |
| --- | --- |
| Quick entry | Choosing an asset and quickly recording one balance at a time |
| Batch | Recording several assets you usually record together, just by typing the amounts |
| By asset | Choosing from the list of assets and checking each asset's records |
| Calendar | Checking the days you recorded on a calendar and recording on a chosen date |

![Input tab](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/input.png)

> **Points**
> - Enter the **balance at that time**, not the amount that was added or removed.
> - Regardless of the number format under **Settings** → **Display Format**, enter amounts in the form "1,234.56" (with a period as the decimal point).
> - For assets with **Treat as Liability** turned on, positive amounts are automatically recorded as negative (liabilities).

## Quick entry: record one at a time

1. On the **Quick entry** tab, tap **Select an asset** at the top and choose the asset from the list of icons.
   You can also choose **Add asset** at the end of the list to add a new asset and record it right away.
2. Enter the date, amount, and other fields (see "Record fields" below).
3. Tap **Save**.

"Recorded to "…"" appears. The screen stays open, so you can choose another asset and keep recording (the amount, memo, and subcategory are cleared, and the date is kept).

![Quick entry](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/input-simple.png)

## Record fields

On Quick entry and the **Add Record** screen, enter the following.

| Field | Description |
| --- | --- |
| Date | The date and time you checked the balance. Tap it to choose a date on the calendar, then a time. The default is the current date and time. |
| Currency | The currency set for the asset (it can't be changed here). |
| Amount | The balance on that date. Thousands separators are added automatically. |
| Exchange rate | Shown only when the asset's currency differs from the default currency. The rate on the record date is filled in automatically (see below). |
| Subcategory (optional) | Choose the type of record (e.g. Salary, Valuation) with the wheel picker. |
| Memo (optional) | Leave a note. You can write multiple lines. |

To close the keyboard, tap an empty area or tap **Done** above the keyboard.

### About the exchange rate

For assets such as foreign currencies, gold, and crypto, an **Exchange rate** field (e.g. 1 USD = … JPY) is shown below the amount.

- At first, the **rate on the record date** is filled in automatically. It is replaced when you change the date or asset.
- You can change it to the rate you actually exchanged at, for example. A rate you enter is used **only to convert this record**; your **Currency & Rates** settings don't change.
- To go back to the automatic rate, tap the ↻ button to the right of the field.

→ [Currencies and Exchange Rates](currency)

## Batch: record several at once

If you always record the same set of assets, for example on payday or at the end of each month, save them as a **batch entry**. Then just type the amounts to record them all at once.

![Batch entry](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/input-batch.png)

### Creating a batch entry

1. On the **Batch** tab, tap **Create batch entry** (you can also create one under **Settings** → **Batch entry**).
2. Set the following.

   | Field | Description |
   | --- | --- |
   | Name | The name of the batch entry (e.g. Month-end balances, Payday). If left blank, it is named "Batch entry". |
   | Sub-category (for all) | The subcategory attached to the records. The same one is attached to every asset. |
   | Assets | Tap **Add assets** to choose the assets to record together. Drag "≡" on the right to reorder them. |

   To use a different subcategory for a single asset, tap the subcategory under that asset and change it.
3. Tap the save button at the top right.

### Recording with a batch entry

1. On the **Batch** tab, tap the batch entry you want to use.
2. Check the **Date** and change it if needed.
3. Enter an amount for each asset. Each field shows the previous amount as "Last …".
   - Tap **Fill blanks with last amounts** to fill the assets you haven't entered yet with their previous amounts. This is handy when some balances haven't changed.
4. Tap **Record …**.

**Assets left blank are not recorded.** Only the assets you entered are recorded, each in its own currency.

### Editing or deleting a batch entry

**Long-press** a batch entry on the **Batch** tab, or tap the pencil icon at the top right of the recording screen, to open the edit screen.
To delete one, tap **Delete this batch entry** at the bottom of the edit screen. Deleting a batch entry doesn't delete records you have already saved.

## By asset: record from the list of assets

The **By asset** tab lists your assets.

- Each asset shows its **latest balance** (in the asset's own currency) and, below it, the **month-over-month change** (the difference from one month ago and the rate of change). Increases are shown in green and decreases in red.
- Assets you excluded from totals are shown dimmed (→ [Managing Assets](assets)).
- Tap an asset to open its record list. Tap **New entry** at the bottom right of the list to open the **Add Record** screen and add a record for that asset.
- Tap **Add asset** at the bottom right to add an asset. Tap the pencil icon at the top right to open **Asset list**, where you can edit, reorder, and delete assets (→ [Managing Assets](assets)).

![By asset](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/input-by-asset.png)

### Reading the record list

![Record list](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/asset-detail.png)

- The **Current Balance** (the amount of the latest record) and the month-over-month change are shown at the top.
- Records are shown in a table with **Date**, **Subcategory**, **Amount**, and **Memo**. Long memos are truncated; tap a record to see the full text.
- You can filter and sort the records as follows.

| Option | Description |
| --- | --- |
| Period | Choose from **1Y** (default), **3Y**, **All**, or **Custom**. For **Custom**, set the start and end dates with the wheel picker. |
| Sort order | Choose from date (newest first), date (oldest first), amount (largest first), or amount (smallest first). |
| Rows per page | Choose how many records to show per page (30, 50, or 100). |

If there are many records, use the page numbers or "‹" and "›" below the table to switch pages. The number of matching records is shown at the top right of the table.

## Calendar: see the days you recorded

The **Calendar** tab shows the days you recorded on a calendar, and lets you add records on a chosen date.

![Calendar](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/input-calendar.png)

- Days with records are marked with a dot: **green if your total assets went up that day, red if they went down**.
- Tap a day to list that day's records (asset name, amount, change from the previous record, and memo) below. Tap a record to edit it.
- Tap **Add a record on this day** to open the **Add Record** screen with that date. You can go back and record on past dates.
- Switch months with the left and right arrows, or by swiping the calendar sideways. Tap the month and year to jump by choosing a year and then a month.
- Choose an asset with the filter icon on the right to show only that asset's records (the dot colors then show that asset's changes).
- Use the button in the middle of the divider between the calendar and the list to collapse the calendar and give the list more room.

## Editing a record

Tap a record in either of the following places to open the **Edit Record** screen. Make your changes and tap **Save**.

- The record list that opens when you tap an asset on the **By asset** tab
- The list of the day's records on the **Calendar** tab

You can't change the asset when editing a record.

## Deleting a record

1. On the **By asset** tab, tap the asset, then tap the edit button (pencil icon) at the top right of the record list.
2. Tap the trash icon on the right of the record you want to delete.
3. When you're done, tap the done button (✓) at the top right.

> **Caution**
> Records are deleted immediately without confirmation and cannot be restored.

## About subcategories

A subcategory is a label you attach to a record. **Sale**, **Withdrawal**, **Salary**, **Valuation**, and **Deposit** are provided at first.
Attaching subcategories lets you see what caused your balance to go up or down in the **Change factors** view of the chart (→ [Viewing Trends in Charts](chart)).
Add, rename, reorder, and delete subcategories under **Settings** → **Subcategories** (→ [Settings](settings)).

## Moving from other apps

You can also import records in bulk from screenshots of banking or brokerage apps, or from CSV files from spreadsheet software.
→ [Data Import (Screenshots and CSV)](data-import)
