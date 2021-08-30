---
lab:
    title: 'Lab: Create and configure a new company'
    module: 'Module 3: Configure Financials'
---

## Exercise 1: Create a new fiscal year

### Scenario

When setting up the company you were misinformed about Contoso’s fiscal year.
Although they want to use Microsoft Dynamics 365 Business Central as of January
1st 2021, their new fiscal year does not start until July 1st 2021.

You will have to correct this mistake and prepare the accounting periods for the
entire fiscal year.

### Tasks

1.  Change the starting date of the fiscal year.

2.  Create accounting periods in bulk.

### Steps

### Task 1

1.  Change the starting date of the fiscal year.

2.  Open the **Accounting Periods** page by clicking on the search icon in the black bar at the top of the page, on the right hand side. After clicking on the search icon type **Acounting Periods**, then click the link to the page.

3.  Select the accounting period with starting date 1/1/2022 and deselect
    the **New Fiscal Year** checkbox.
    **Note:** You will need to click the **Edit list** button to deselect the check box.

4.  Select the accounting period with starting date 7/1/2021 and select the
    **New Fiscal Year** checkbox.

5.  Leave the selection on the **New Fiscal Year** checkbox for the
    accounting period with starting date 1/1/2021.

### Task 2

1.  Create accounting periods in bulk.

7.  In the **Accounting Periods** page, select **More options**, select **Actions** and then select
    **Create Year**.

8.  On the window that opens, fill in the following options:

       1.  In the **Starting Date** field, enter 1/1/2022.

       2.  In the **No. of Periods** field, enter ‘6’.

       3.  In the **Period Length** field, enter 1M.

9.  Click **OK**.

10.  New accounting periods are now created, where the last accounting period
    has a starting date of 7/1/2022 and the **New Fiscal Year** checkbox is
    selected.

## Exercise 2: Configure the general ledger setup

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
transactions for January 2021, but also allow your own user to process the
opening balance on December 31st 2020.

### Tasks

1.  Determine the local currency.

2.  Set up global and shortcut dimensions.

3.  Allow posting in the open accounting period.

### Steps

### Task 1

Determine the local currency.

1.  Open the **General Ledger Setup** page by clicking on the search icon in the black bar at the top of the page, on the right hand side. After clicking on the search icon type **General Ledger Setup**, then click the link to the page.

3.  In the **General** FastTab review that the following fields regarding
    local currency are filled in correctly.

       1.  The **LCY Code** field must be set to USD.

       2.  The **Local Currency Symbol** field must contain the $ symbol.

       3.  The **Local Currency Description** field must be filled in with ‘US
            dollar’

4.  In the **General** FastTab review that the following fields regarding
    local currency rounding are filled in correctly:

       1.  The **Amount Decimal Places ($)** field must be set to 2:2.

       2.  The **Unit-Amount Decimal Places ($)** field must be set to 2:5.

### Task 2

Set up global and shortcut dimensions.

1.  In the **General Ledger Setup** page, select **More options**, then select **Actions**, then
    **Functions** and then **Change Global Dimensions**.

7.  In the **Change Global Dimensions** page, fill in the following fields:

       1.  In the **Global Dimension 1 Code** field select the value
            SALESPERSON.

       2.  In the **Global Dimension 2 Code** field leave the value CUSTOMER
            GROUP.

8.  Select **Sequential** and then click **Start**.

9.  Close the **Change Global Dimensions** page.

10.  In the **General Ledger Setup** page, in the **Dimensions** FastTab, in
    the **Shortcut Dimension 3 Code** field select the value DEPARTMENT (**Note:** You may need to click the 'Show more' option to expand the fields visible)

### Task 3

Allow posting in the open accounting period.

1.  In the **General Ledger Setup** page, in the **General** FastTab, fill
    in the following fields:

       1.  In the **Allow Posting From** field, select 1/1/2021.

       2.  In the **Allow Posting To** field, select 1/31/2021.

13.  Close the **General Ledger Setup** page.

14.  Open the **User Setup** page by clicking on the search icon in the black bar at the top of the page, on the right hand side. After clicking on the search icon type **User Setup**, then click the link to the page.

16.  Select **+ New**.

15.  In the **User ID** field, enter your own user id.

16.  In the **Allow Posting From** field, enter 12/31/2020.
