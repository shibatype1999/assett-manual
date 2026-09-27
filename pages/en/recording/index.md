# Recording Balances
<!-- position: 3 -->
<!-- description: How to record, edit, and delete balances for each asset, and how to read the record list. -->

## The Input tab

The **Input** tab (titled **Asset input**) lists the assets you have registered.

![Input tab](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/input.png)

- Each asset shows its **latest balance** (in the asset's own currency) and, below it, the **change vs last month** (amount and percentage). Increases are shown in green and decreases in red.
- Tap an asset to open its record list.
- Tap **Add asset** at the bottom right to add an asset. Tap the pencil icon at the top right to open the **Asset list**, where you can edit, reorder, and delete assets (→ [Managing Assets](assets)).

## Recording a balance

1. On the **Input** tab, tap the asset you want to record.
2. Tap **New entry** at the bottom right.
3. On the **Add Record** screen, fill in the following:

   | Field | Description |
   | --- | --- |
   | Date | The date and time you checked the balance. Tap to pick a date from the calendar, then a time. Defaults to now. |
   | Currency | Shows the currency set for the asset (cannot be changed here). |
   | Amount | The balance as of that date. Thousands separators are added automatically. |
   | Subcategory (optional) | Choose a label for the record (e.g. Salary, Valuation) with the scroll wheel. |
   | Memo (optional) | Any note you like. You can write multiple lines. |

4. Tap **Save** at the top right.

![Add Record screen](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/record-form.png)

> **Notes**
> - Enter the **balance at that time**, not the amount that increased or decreased.
> - Regardless of the number format in **Settings** → **Display Format**, enter amounts like "1,234.56" (with a period as the decimal point).
> - In an asset with **Treat as Liability** turned on, amounts are recorded as negative (liability) even if you enter a positive number.

## Reading the record list

Tap an asset to see its record list.

![Record list](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/asset-detail.png)

- **Current Balance** (the amount of the latest record) and the change vs last month are shown at the top.
- Records are shown in a table of **Date**, **Subcategory**, **Amount**, and **Memo**. Long memos are shortened; tap the record to see the full text.
- You can filter and sort the records as follows.

| Control | Description |
| --- | --- |
| Period | Choose **1Y** (default), **3 years**, **All**, or **Custom**. With **Custom**, set the start and end dates with the scroll wheels. |
| Sort | Choose **Date (newest)**, **Date (oldest)**, **Amount (high to low)**, or **Amount (low to high)**. |
| Per page | Choose how many records to show per page (30, 50, or 100). |

If there are many records, use the page numbers or **‹** / **›** below the table. The number of matching records is shown above the table.

## Editing a record

1. In the record list, tap the record you want to edit.
2. On the **Edit Record** screen, make your changes and tap **Save**.

## Deleting a record

1. Tap the edit button (pencil icon) at the top right of the record list.
2. Tap the trash icon to the right of the record you want to delete.
3. When you're done, tap the done button (✓) at the top right.

> **Caution**
> Records are deleted immediately without confirmation and cannot be restored.

## About subcategories

Subcategories are labels you can attach to records. **Sale**, **Withdrawal**, **Salary**, **Valuation**, and **Deposit** are provided by default.
If you attach subcategories, the **Change factors** view in the chart shows what caused your balances to rise or fall (→ [Viewing Trends in Charts](chart)).
You can add, rename, reorder, and delete subcategories under **Settings** → **Subcategories** (→ [Settings](settings)).
