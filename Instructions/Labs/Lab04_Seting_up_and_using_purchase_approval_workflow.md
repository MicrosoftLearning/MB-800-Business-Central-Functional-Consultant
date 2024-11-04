Hands-on-Lab 04: Setting up and using a purchase approval workflow
===========================================
### Scenario

When setting up the company you were misinformed about Contoso’s fiscal year.
Although they want to use Microsoft Dynamics 365 Business Central as of January
1st 2022, their new fiscal year does not start until July 1st 2022.

You will have to correct this mistake and prepare the accounting periods for the
entire fiscal year.

### Tasks

1.  Change the starting date of the fiscal year.

2.  Create accounting periods in bulk.

### Steps

1.  Change the starting date of the fiscal year.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Accounting periods`, and then choose the related link.

    2.  Open the **Accounting Periods** page.

    3.  Select the accounting period with starting date **7/1/2022** and select
        the **New Fiscal Year** checkbox.

    4.  Leave the selection on the **New Fiscal Year** checkbox for the
        accounting period with starting date **1/1/2022**.

2.  Create accounting periods in bulk.

    1.  In the **Accounting Periods** page, select **Create Year**.

    2.  On the window that opens, fill in the following options:

        1.  In the **Starting Date** field, enter `7/1/2022`.

        2.  In the **No. of Periods** field, enter `12`.

        3.  In the **Period Length** field, enter `1M`.

    3.  Click **OK**.

    4.  New accounting periods are now created, where the last accounting period
        has a starting date of **7/1/2023** and the **New Fiscal Year** checkbox
        is selected.

Exercise 2: Configure the general ledger setup
----------------------------------------------

### Scenario

After setting up the correct accounting periods, you will complete some general
accounting setup.

Contoso is located in the United States and will record their accounting data in
US dollar, thereby respecting the currencies 2 digit decimals for displaying
invoice amounts and amounts. Unit-prices however, can be shown with 2 up to 5
digit decimals.

Analysis of recorded accounting data will be mainly focused on the sales
transactions, using the created dimensions. Contoso’s accounting manager would
like to analyze these sales transactions directly from the chart of accounts, to
make sure all the detailed information is at hand. Later they will set up some
more general reports. He would also like to track costs by department where, for
now, the main focus is on easily entering this information. The specific
reporting details will be determined later on.

Once the company’s users will start to record sales and purchase transactions,
the accounting manager wants to make sure they are only processed within the
current accounting period. Make sure the company is set for the first
transactions for January 2022, but also allow your own user to process the
opening balance on December 31st 2021.

### Tasks

1.  Determine the local currency.

2.  Set up global and shortcut dimensions.

3.  Allow posting in the open accounting period.

### Steps

1.  Determine the local currency.

    1.  Select the Search icon in the top-right corner of the page,
        enter `General Ledger Setup` and then choose the related link.

    2.  Open the **General Ledger Setup** page.

    3.  In the **General** FastTab review that the following fields regarding
        local currency are filled in correctly.

        1.  The **LCY Code** field must be set to USD.

        2.  The **Local Currency Symbol** field must contain the \$ symbol.

        3.  The **Local Currency Description** field must be filled in with ‘US
            dollar’

    4.  In the **General** FastTab review that the following fields regarding
        local currency rounding are filled in correctly:

        1.  The **Amount Decimal Places (\$)** field must be set to 2:2.

        2.  The **Unit-Amount Decimal Places (\$)** field must be set to 2:5.

2.  Set up global and shortcut dimensions.

    1.  In the **General Ledger Setup** page, select **Change Global Dimensions**.

    2.  In the **Change Global Dimensions** page, fill in the following fields:

        1.  In the **Global Dimension 1 Code** field select the value
            **SALESPERSON_NEWLIST**.

        2.  In the **Global Dimension 2 Code** field leave the value **CUSTOMER
            GROUP**.

    3.  Select **Sequential** and then click **Start**.

    4.  Close the **Change Global Dimensions** page.

    5.  In the **General Ledger Setup** page, in the **Dimensions** FastTab,
        click **Show more**. In the **Shortcut Dimension 3 Code** field select
        the value **DEPARTMENT**.

3.  Allow posting in the open accounting period.

    1.  In the **General Ledger Setup** page, in the **General** FastTab, fill
        in the following fields:

        1.  In the **Allow Posting From** field, select **1/1/2022**.

        2.  In the **Allow Posting To** field, select **1/31/2022**.

    2.  Close the **General Ledger Setup** page.

    3.  Select the Search icon in the top-right corner of the page,
        enter `User Setup` and then choose the related link.

    4.  In the **User Setup** page, select **+ New**.

    5.  In the **User ID** field, enter your own user id.

    6.  In the **Allow Posting From** field, enter **12/31/2021**.
