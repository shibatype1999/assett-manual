# Currencies and Exchange Rates
<!-- position: 8 -->
<!-- description: Default currency, automatic and manual exchange rates, and custom currencies such as points and miles. -->

You can set a currency for each asset. Total assets and charts are always shown in your **default currency**.

Currency settings are under **Settings** → **Currency & Rates**.

![Currency & Rates screen](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/currency-settings.png)

## Available currencies

| Type | Currencies |
| --- | --- |
| Fiat currencies | Japanese Yen, US Dollar, Euro, British Pound, Australian Dollar, Canadian Dollar, Swiss Franc, Chinese Yuan, Hong Kong Dollar, Taiwan Dollar, South Korean Won, Indian Rupee, Indonesian Rupiah, Brazilian Real, Singapore Dollar, New Zealand Dollar, Qatari Riyal, Saudi Riyal, UAE Dirham, Malaysian Ringgit, Thai Baht, Turkish Lira, Russian Ruble |
| Gold | Gold (g), Gold (ozt) |
| Crypto | Bitcoin, Ethereum |
| Custom currencies | Points and Miles (registered from the start), plus currencies you add yourself |

Gold, crypto, points, and miles are recorded as a **quantity** (e.g. 10 g, 0.5 BTC, 3,000 pt) rather than a monetary amount.

## Setting the default currency

The default currency is used to show your total assets, charts, and asset goal. It is also the initial currency for new assets.

1. Open **Settings** → **Currency & Rates**.
2. Tap the **Default Currency** field.
3. Choose a currency with the scroll wheel, then tap **Save**.

If you choose **Follow system setting**, a currency based on your device's language is used (for example, US Dollar for English and Japanese Yen for Japanese).

> **Caution**
> If you change the default currency when you already have records, a confirmation appears.
> The exchange rates saved with each record (see below) are for the previous default currency, so they can no longer be used. Past totals and charts are recalculated with the historical rates available, so they may differ from before or may not be shown correctly.

## Automatic exchange rates

If any asset uses a currency other than your default currency, the app fetches the latest rates from the internet to convert amounts.

- Rates are fetched automatically when the app starts.
- They are also fetched when you pull down on the **Dashboard**.
- Automatic fetching happens **up to 2 times per day**. When the limit is reached, "Reached today's limit (up to 2 times per day)" is shown.
- Tap **Refresh rates** to the right of **Currency Rates** on the **Currency & Rates** screen to fetch the rates of all the currencies you use again.
- Rates for custom currencies (including points and miles) are not fetched automatically. Set them manually.
- If the app can't connect to the internet, it uses the rates it fetched last time or built-in reference rates.

### Historical rates

When charts and asset composition show amounts for past dates, they are converted with **the rate on that date**.
Historical rates come from data bundled in the app, based on published statistics, and from rates fetched for the periods needed. The sources are shown at the bottom of the **Currency & Rates** screen.
For currencies and periods without historical rates, the exchange rate saved with each record or the current rate is used.

Add the **Exchange rates** panel to the dashboard to see the rates of the currencies you use and the last update time (→ [Dashboard](dashboard)).

## Setting rates manually

The **Currency Rates** section of the **Currency & Rates** screen lists the non-default currencies used by your assets.

![Currency Rates](https://raw.githubusercontent.com/shibatype1999/assett-manual/main/images/en/currency-rate-row.png)

1. In the field labeled like "1 USD → JPY", enter how much one unit is worth in your default currency.
2. Tap ✓ on the right to save.

To go back to the latest rates, tap **Refresh rates** to the right of the heading. If fetching fails, enter the rate manually.

Set rates for custom currencies the same way in the **Custom Currency Rates** section below.

## Exchange rate for each record

When you record a balance for an asset in a foreign currency or the like, the record screen shows an **Exchange rate** field filled with **the rate on the record date**.

- If you change it, for example to the rate you actually exchanged at, that rate is used **only to convert that record on its date**. It doesn't affect your **Currency & Rates** settings or conversions on other dates.
- Your current total assets are converted with current rates, not with the rates saved with records.

→ [Recording Balances](recording)

## Gold valuation

If you have gold (g or ozt) assets, **Gold valuation** appears below **Currency Rates**. The gold rate is the international spot price; use these settings to bring it closer to dealer prices, for example.

| Item | Description |
| --- | --- |
| Include Japanese consumption tax (10%) | When on, gold is valued at tax-inclusive prices, as Japanese dealers quote them. |
| Markup | Add dealer premiums or fees (spot price + n%). Tap ✓ on the right to save. |

The price actually used is shown, for example "Price used: 1 g = … (spot × …)".

## Custom currencies

Currencies that are not in the list, as well as points and miles, are handled as "custom currencies".

- **Points** and **Miles** are registered from the start. They cannot be deleted, but you can change their name, unit, and rate. They are initially converted as 1 pt = 1 JPY and 1 mi = 1 JPY, so change them to match the value you assign to them.
- Custom currencies can be chosen as an asset's currency.

### Adding a custom currency

1. On the **Currency & Rates** screen, tap **Add Custom Currency**.
2. Fill in the following:

   | Field | Description |
   | --- | --- |
   | Display Name | The name of the currency. |
   | Currency Code | A code to identify the currency (e.g. MYCOIN). It must not match any other currency, and it cannot be changed after the currency is added. |
   | Unit | The unit shown after amounts (e.g. miles). If left blank, the code is shown. |
   | Rate | How much one unit is worth in your default currency. **Required** (a number greater than 0). |

3. Tap **Save**.

### Editing, reordering, and deleting custom currencies

- **Edit** – Tap a row in the list.
- **Reorder** – Press and hold the **≡** handle on the right, then drag it up or down.
- **Delete** – Tap the pencil icon to the right of the **Custom Currencies** heading, tap the trash icon, then tap **Delete** in the confirmation dialog.

> **Caution**
> A custom currency used by an asset can't be deleted. If you try, the names of the assets using it are shown. Change the currency of those assets first.

## If "Some currency rates could not be fetched and are not included in the total" appears

If an asset uses a currency whose rate is unknown, its amount is not included in your total assets.
Fetch the rate for that currency on the **Currency & Rates** screen, or enter it manually.
