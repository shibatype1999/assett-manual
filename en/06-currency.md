# Currencies and Exchange Rates

You can set a currency for each category. Total assets and charts are always shown in your **default currency**.

Currency settings are under **Settings** → **Currency & Rates**.

![Currency & Rates screen](../images/en/currency-settings.png)

## Available currencies

| Type | Currencies |
| --- | --- |
| Fiat currencies | Japanese Yen, US Dollar, Euro, British Pound, Australian Dollar, Canadian Dollar, Swiss Franc, Chinese Yuan, Hong Kong Dollar, South Korean Won, Indian Rupee, Indonesian Rupiah, Brazilian Real, Singapore Dollar, New Zealand Dollar, Qatari Riyal, Saudi Riyal, UAE Dirham, Malaysian Ringgit, Thai Baht, Turkish Lira, Russian Ruble |
| Gold | Gold (g), Gold (ozt) |
| Crypto | Bitcoin, Ethereum |
| Points, etc. | Points, Miles |
| Custom currencies | Currencies you add yourself (see below) |

Gold, crypto, points, and miles are recorded as a **quantity** (e.g. 10 g, 0.5 BTC, 3,000 pt) rather than a monetary amount.

## Setting the default currency

The default currency is used to show your total assets, charts, and asset goal.

1. Open **Settings** → **Currency & Rates**.
2. Tap the **Default Currency** field.
3. Choose a currency with the scroll wheel, then tap **Save**.

If you choose **Follow system setting**, a currency based on your device's language is used (for example, US Dollar for English and Japanese Yen for Japanese).

## Automatic exchange rates

If any category uses a currency other than your default currency, the app fetches the latest rates from the internet to convert amounts.

- Rates are fetched automatically when the app starts.
- You can also fetch them with the refresh button (⟳) at the top right of Total Assets on the **Input** tab.
- Rates can be fetched **up to 2 times per day**. When the limit is reached, "Reached today's limit (up to 2 times per day)" is shown.
- Rates for points, miles, and custom currencies are not fetched automatically. Set them manually.
- If the app can't connect to the internet, it uses built-in reference rates or the rates it fetched last time.

## Setting rates manually

The **Currency Rates** section of the **Currency & Rates** screen lists the non-default currencies used by your categories, as well as your custom currencies.

![Currency Rates](../images/en/currency-rate-row.png)

1. In the field labeled like "1 USD → JPY", enter how much one unit is worth in your default currency.
2. Tap ✓ on the right to save.

Tap the ⟳ button next to the field to fetch the latest rate for that currency into the field (this counts toward the limit of 2 times per day). If fetching fails, enter the rate manually.

> **Note**
> Points and miles are initially converted as 1 pt = 1 JPY and 1 mi = 1 JPY. Change them to match the value you assign to them.

## Adding a custom currency

You can add currencies that are not in the list, or your own points, as custom currencies.

1. On the **Currency & Rates** screen, tap **Add Custom Currency**.
2. Fill in the following:

   | Field | Description |
   | --- | --- |
   | Display Name | The name of the currency. |
   | Currency Code | A code to identify the currency (e.g. MYCOIN). It must not match any other currency, and it cannot be changed after the currency is added. |
   | Unit | The unit shown after amounts (e.g. Miles). If left blank, the code is shown. |
   | Rate | How much one unit is worth in your default currency. Defaults to 1 if left blank. |

3. Tap **Save**.

Once added, the custom currency can be selected as a category currency.
Use the pencil icon in the list to edit it, or the trash icon to delete it.

> **Caution**
> Custom currencies are deleted immediately without confirmation. If you delete a custom currency that is in use, amounts in that category may no longer be converted correctly.

## If "Some currency rates could not be fetched and are not included in the total" appears

If a category uses a currency whose rate is unknown, its amount is not included in your total assets.
Fetch the rate for that currency on the **Currency & Rates** screen, or enter it manually.
