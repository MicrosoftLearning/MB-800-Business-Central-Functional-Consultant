
---
lab:
    title: 'Lab: Set up currencies'
    module: 'Module 3: Configure Financials'
---

Hands-on-Lab 3.6: Set up currencies
===================================

Exercise 1: Set up currencies
-----------------------------

### Scenario

Since Contoso is engaging in foreign sales activities in Europe, as well as
importing their products from export countries, they are in need of working with
different currencies throughout the Business Central database.

You will make sure the following foreign currencies are set up correctly:

-   EUR = Euro – at the beginning of January 1st, 2022, the relational exchange
    rate amount between EUR and LCY is 100 EUR = 113 USD.

-   CAD = Canadian dollar – at the beginning of January 1st, 2022, the
    relational exchange rate amount between CAD and LCY is 100 CAD = 78 USD

The currency exchange rates will be updated on a regular basis, however when
working in the Business Central database, users should be able to adjust the LCY
exchange rate on a transactional level.

These currencies follow the same rules regarding decimal places and roundings as
the LCY, meaning that the currencies show 2 digit decimals for displaying
invoice amounts and amounts, whereas the unit-prices can be shown with 2 up to 5
digit decimals.

Any gains and losses coming from currency exchange rate differences are posted
onto the 40500 g/l account.

*Remark: Throughout the labs in Module 5 – Operations, multicurrency will be
used and a separate lab for updating the currency exchange rate is created.*

### Tasks

1.  Set up a foreign currency.

2.  Determine currency exchange rates.

### Steps

1.  Set up a foreign currency.

    1.  Open the **Currencies** page.

    2.  Select the Euro currency and review that the following fields are filled
        in correctly.

        1.  The **Code** field must be set to EUR.

        2.  The **Description** field must be filled in with ‘Euro’.

        3.  The **ISO Code** must be filled in with EUR.

        4.  The **Symbol** field must contain the € symbol.

        5.  The **Realized Gains Acc.**, **Realized Losses Acc.**, **Unrealized
            Gains Acc.** and **Unrealized Losses Acc.** fields must all be
            filled in with ‘40500’.

        6.  The **Amount Decimal Places** field must be set to 2:2.

        7.  The **Unit-Amount Decimal Places** field must be set to 2:5.

    3.  Select the Canadian dollar currency and review that the following fields
        are filled in correctly.

        1.  The **Code** field must be set to CAD.

        2.  The **Description** field must be filled in with ‘Canadian dollar’.

        3.  The **ISO Code** must be filled in with CAD.

        4.  The **Symbol** field must contain the $ symbol.

        5.  The **Realized Gains Acc.**, **Realized Losses Acc.**, **Unrealized
            Gains Acc.** and **Unrealized Losses Acc.** fields must all be
            filled in with ‘40500’.

        6.  The **Amount Decimal Places** field must be set to 2:2.

        7.  The **Unit-Amount Decimal Places** field must be set to 2:5.

2.  Determine currency exchange rates.

    1.  In the **Currencies** page, select the Euro currency.
    
    2. Select **More options**, select **Actions**, and then select **Exch. Rates**.

    3.  In the opened **Currency Exchange Rates** page, select **New** and fill
        in the following fields:

        1.  In the **Starting Date** field, enter 1/1/2022.

        2.  In the **Currency Code** field, enter EUR.

        3.  Leave the **Relational Currency Code** field blank.

        4.  In the **Exchange Rate Amount** field and the **Adjustment Exch.
            Rate Amount** field, enter ‘100’.

        5.  In the **Relational Exch. Rate Amount** field and the **Relational
            Adjmt Exch Rate Amt** field, enter ‘113’.

        6.  In the **Fix Exchange Rate Amount**, leave the default value
            ‘Currency’.

    4.  Close the **Currency Exchange Rates** page.

    5.  In the **Currencies** page, select the Canadian dollar currency.

    6. Select **More options**, select **Actions**, and then select **Exch. Rates**.

    7.  In the opened **Currency Exchange Rates** page, select **New** and fill
        in the following fields:

        1.  In the **Starting Date** field, enter 1/1/2022.

        2.  In the **Currency Code** field, enter CAD.

        3.  Leave the **Relational Currency Code** field blank.

        4.  In the **Exchange Rate Amount** field and the **Adjustment Exch.
            Rate Amount** field, enter ‘100’.

        5.  In the **Relational Exch. Rate Amount** field and the **Relational
            Adjmt Exch Rate Amt** field, enter ‘78’.

        6.  In the **Fix Exchange Rate Amount**, leave the default value
            ‘Currency’.
