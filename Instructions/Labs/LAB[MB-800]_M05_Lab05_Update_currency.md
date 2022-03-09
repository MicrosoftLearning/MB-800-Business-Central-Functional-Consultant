
---
lab:
    title: 'Lab: Update currency exchange rate'
    module: 'Module 5: Operations'
---

Hands-on-Lab 5.5: Update currency exchange rate
===============================================

Exercise 1: Update the CAD:USD currency exchange rate
-----------------------------------------------------

### Scenario

At the end of January 2022, the relational exchange rate amount between CAD and
LCY is 100 CAD = 79 USD. Because there are customers and vendors that use CAD as
their default currency, you must run the Adjust Exchange Rates batch job.

Because you posted activity to its account this month, you want to trace any
adjustment to the vendor ledger entry for vendor OakvilleWorld.

*Remark: to successfully complete this lab, first the lab 5.1 Process purchase –
exercise 4 needs to be completed*

##### **High Level Steps**

### Tasks

1.  Determine currency exchange rates

2.  Run the Adjust Exchange Rates batch job

### Steps

1.  Determine currency exchange rates.

    1.  In the **Currencies** page, select the CAD currency.

    2.  Select **Actions**, and then select **Exch. Rates**.

    3.  In the opened **Currency Exchange Rates** page, select **New** and fill
        in the following fields:

        1.  In the **Starting Date** field, enter 1/31/2022.

        2.  In the **Currency Code** field, enter CAD.

        3.  Leave the **Relational Currency Code** field blank.

        4.  In the **Exchange Rate Amount** field and the **Adjustment Exch.
            Rate Amount** field, enter ‘100’.

        5.  In the **Relational Exch. Rate Amount** field and the **Relational
            Adjmt Exch Rate Amt** field, enter ‘79’.

        6.  In the **Fix Exchange Rate Amount**, leave the default value
            ‘Currency’.

    4.  Close the **Currency Exchange Rates** page.

2.  Run the Adjust Exchange Rates batch job.

    1.  In the **Currencies** page, select **Actions** and then select **Adjust
        Exchange Rate.**

    2.  On the **Options** FastTab, fill in the following fields:

        1.  Leave the **Starting Date** field blank so that all transactions are
            included.

        2.  In the **Ending Date** field, enter 1/31/2022.

        3.  Accept the default settings in the **Posting Description** and
            **Posting Date** fields.

        4.  In the **Document Number** field, enter ADJCAD-0122.

        5.  Select the **Adjust Customer**, **Adjust Vendor** and **Adjust Bank
            Accounts** checkboxes.

    3.  On the **Filter:Currency** FastTab, fill in the following fields:

        1.  In the **Code** field, enter CAD.

    4.  Click **OK**.

3.  Review the vendor ledger entry for OakvilleWorld.

    1.  On the **Vendors** list page, select vendor OakvilleWorld (V9007).

    2.  Select **Manage** and then select **Edit**.

    3.  On the opened vendor card, select **Related**, then select **History**,
        and then **Ledger Entries**.

    4.  On the **Vendor Ledger Entries** page, select the invoice with external
        document no. OW-21-M2458.

    5.  Select **Entry**, and then select **Detailed Ledger Entries**.

    6.  There are two detailed customer ledger entries:

        1.  One for the initial entry.

        2.  One for the unrealized gain.

![](https://github.com/MicrosoftLearning/MB-800-Business-Central-Functional-Consultant/blob/master/Instructions/Labs/media/MB800_2021_Lab%205.5_detailed_customer_ledger_entries.png)

1.  Close the **Detailed Ledger Entries** page.

2.  Close the **Customer Ledger Entries** page.
