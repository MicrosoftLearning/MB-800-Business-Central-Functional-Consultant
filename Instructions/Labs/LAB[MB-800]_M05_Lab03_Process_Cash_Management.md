---
lab:
    title: 'Lab: Process Cash Management'
    module: 'Module 5: Operations'
---

## Exercise 1: Create and post journal entries

### Scenario

As the functional consultant you have prepared a configuration package for the
import of the opening balance.

The excel file contains all journal lines for all balance sheet accounts and is
prepared in the OPENING general journal, with the BALANCE journal batch,
containing dimension information.

The accounting manager at Contoso has provided you with the following opening
balance to be posted on December 31st, 2020.

![](media/12e7fce33cdf64c933410a7ef8f85296.png)

### Tasks

1.  Prepare the journal for the G/L opening balance.

2.  Create and export a configuration package including dimension information.

3.  Prepare data in excel.

4.  Import and apply the configuration package.

5.  Post the general journal.

### Steps

1.  Prepare the journal for the G/L opening balance.

    1.  First make sure your work date is set to 31/12/2020.

    2.  On the general journals list page, select the OPENING journal.

    3.  Open the assist edit button to the right of the **Batch Name** field.

        1.  Select the BALANCE journal batch.

        2.  Click **OK**.

    4.  Select **Actions**, then select **Opening Balance**, then select
        **Prepare journal** and then select **G/L Accounts Opening Balance**.

    5.  The journal lines are automatically filled in for all balance accounts.

2.  Create and export a configuration package including dimension information.

    1.  In the **Configuration Packages** page, click **New** to create a new
        configuration package.

    2.  In the **Code** field, enter OPENING.

    3.  In the **Package Name** field, enter Opening Balances.

    4.  On the **Tables** section of the Config. Package Card, enter a new line
        as follows.

    5.  Open the assist edit button to the right of the **Table ID** field.

    6.  In the window that opens, select the **Gen. Journal Line** table and
        click **OK**.

    7.  Then press ENTER or TAB.

    8.  You will be asked to check related tables, click **No**.

    9.  Make sure the general journal line table line is selected.

    10. Select the **Dimensions as Columns** checkbox.

    11. Select the **Delete Table Records Before Processing** checkbox.

    12. Select **Table** and then **Fields**.

    13. On the field list page, first select **Clear Included**, to deselect the
        **Include Field** checkbox for all the fields.

    14. Then select the **Include Field** checkbox for the following fields:

        1.  Account Type

        2.  Account No.

        3.  Posting Date

        4.  Document Type

        5.  Document No.

        6.  Description

        7.  Currency Code

        8.  Amount

        9.  Amount (LCY)

        10. Document Date

        11. External Document No.

    15. The **Validate Field** checkbox is automatically selected.

    16. Click **Close**.

    17. In the **Config. Package Card** page, select **Actions**, then
        **Package**, and then **Export to Excel**.

    18. Click **Yes** to export the configuration package.

3.  Prepare data in excel.

    1.  Open the exported excel file from the download folder.

    2.  Delete the lines that are exported to Excel, so that you can start from
        a blank Excel template.

    3.  Enter the information as provided by Contoso.

    4.  Save the excel file.

4.  Import and apply the configuration package.

    1.  In the **Configuration Packages** page, select the new configuration
        package for opening balances and select **Manage** and then **Edit**.

    2.  In the **Config. Package Card** page, select **Actions**, then select
        **Package**, and then **Import from Excel**.

    3.  Click **Choose…** and select the excel file.

    4.  Click **Open**.

    5.  In the preview page, select **Import**.

    6.  In the **Config. Package Card** page, select **Actions**, then select
        **Functions**, and then **Apply Package**.

    7.  Click **Yes**.

5.  Post the general journal.

    1.  Make sure the **Allow Posting From** field, on the **General Ledger
        Setup** page, is set to 12/31/2020.

    2.  On the general journals list page, select the OPENING journal.

    3.  Open the assist edit button to the right of the **Batch Name** field.

        1.  Select the BALANCE journal batch.

        2.  Click **OK**.

    4.  Select **Post/Print**, and then select **Post**.

    5.  Click **Yes**.

## Exercise 2: Create and post journal entries

### Scenario

The accounting manager at Contoso also provided you with the open customer and
vendor ledger entries.

You receive the configuration package, that you can import into the correct
general journals, review and post.

![](media/d426bb5bb9eec9b6284bb2acd13fd889.png)

*(Remark: if you do not have the configuration package for this lab, you can use
the configuration package from exercise 1 and use the excel sheet to import
these opening ledger entries)*

### Tasks

1.  Import and apply a predefined package containing historical data (customer
    and vendor open entries).

2.  Post the general journal.

### Steps

1.  Import and apply a predefined package containing historical data (customer
    and vendor open entries).

    1.  On the **Configuation Packages** page, select **Process** and then
        select **Import Package**.

    2.  Click **Choose…** and select the rapidstart package for Lab 5.3.

    3.  Click **Open**.

    4.  In the preview page, select **Import**.

    5.  In the **Config. Package Card** page, select **Actions**, then select
        **Functions** and then **Apply Package**.

    6.  Click **Yes**.

2.  Post the general journal.

    1.  On the general journals list page, select the OPENING journal.

    2.  Open the assist edit button to the right of the **Batch Name** field.

        1.  Select the CUST journal batch.

        2.  Click **OK**.

    3.  Select **Post/Print**, and then select **Post**.

    4.  Click **Yes**.

    5.  Open the assist edit button to the right of the **Batch Name** field.

        1.  Select the VEND journal batch.

        2.  Click **OK**.

    6.  Select **Post/Print**, and then select **Post**.

    7.  Click **Yes**.

## Exercise 3: Process vendor payments

### Scenario

At the end of each month all euro payments are transferred from the EUROP bank
account to the European vendors, using an electronic SEPA file. Each time a
payment is performed a new payment journal batch is created.

Vendor PURE-LOOK has recently changed their bank account and has asked you to
make sure the next euro payment will be done on that Belgian account. They also
request to be paid for all invoices as a single payment.

The bank account details: SNS - IBAN: BE67 2900 0461 4187 - SWIFT Code: BBRUBEBB

The first payment to this vendor V9005 will be performed on January 31st, 2021,
using the EUROP payment journal, with a new batch PAY1.

### Tasks

1.  Create a vendor bank account.

2.  Suggest vendor payments.

3.  Process payment journals.

### Steps

1.  Create a vendor bank account.

    1.  On the **Vendors** list page, select vendor PURE-LOOK.

    2.  Select **Manage** and then select **Edit**.

    3.  On the vendor card, go to the **Invoicing** Fast Tab.

    4.  In the **Preferred Bank Account Code** field, click on the Look Up Value
        button and click **New**.

    5.  On the opened vendor bank account card, fill in the following fields:

        1.  On the **General** FastTab, fill in the following fields:

            1.  In the **Code** field, enter SNS.

            2.  In the **Name** field, enter ‘Pure-Look’.

            3.  In the **Country/Region Code** field, enter BE.

            4.  In the **Currency Code** field, enter EUR.

        2.  On the **Transfer** FastTab, fill in the following fields:

            1.  In the **SWIFT Code** field, enter BBRUBEBB.

            2.  In the **IBAN** field, enter BE67290004614187.

            3.  Select the **Use for Electronic Payments** checkbox.

        3.  Click **OK**.

    6.  The new vendor bank account is automatically filled in in the
        **Preferred Bank Account Code** field on the vendor card.

2.  Suggest vendor payments.

    1.  On the payment journals list page, select the EUROP journal.

    2.  Open the assist edit button to the right of the **Batch Name** field.

    3.  On the opened **General Journal Batches** page, click **New** and fill
        in the following fields:

        1.  In the **Name** field, enter PAY1.

        2.  In the **Description** field, enter ‘Payment January 2021’.

        3.  In the **Bal. Account Type** field, enter Bank Account.

        4.  In the **Bal. Account No.** field, enter EUROP.

        5.  In the **No. Series** field, the value GJNL-PMT is automatically
            filled in.

        6.  Click **OK**.

    4.  The new batch PAY1, is automatically filled in in the **Batch Name**
        field on the payment journal.

    5.  Select **Prepare**, and then select **Suggest Vendor Payments**.

        1.  On the **Options** FastTab, fill in the following fields:

            1.  In the **Last Payment Date** field, enter 1/31/2021.

            2.  Leave the **Check Other Journal Batches** checkbox selected.

            3.  Select the **Summarize per Vendor** checkbox.

        2.  On the **Filter:Vendor** FastTab, in the **No**. filter, enter
            V9005.

        3.  Click **OK** to perform the batch job and automatically fill in the
            lines in the payment journal.

3.  Process payment journals.

    1.  Select **Bank**, and then select **Export**.

    2.  Select **Post/Print**, and then select **Post**.

## Exercise 4: Process customer payments

### Scenario

On January 24th, 2021, Contoso receives a \$ 45,678.14 payment from customer
C00010 Spotsmeyer’s Furnishings on their CHECKINGS bank account.

This payment is for all open invoices from the previous month:

-   S20/12/0976 - \$ 1,087.12

-   S20/12/1576 - \$ 2,687.68

-   S20/12/2687 - \$ 3,000.00

You need to process this payment using the Payment Registration by applying the
invoices.

### Tasks

1.  Review payment registration setup.

2.  Process payment registrations.

### Steps

1.  Review payment registration setup.

    1.  On the **Payment Registration Setup** page, make sure following fields
        are entered.

        1.  In the **Journal Template Name** field, enter CASHRCPT.

        2.  In the **Journal Batch Name** field, enter GENERAL.

        3.  In the **Balancing Account Type** field, enter Bank Account.

        4.  In the **Balancing Account** field, enter CHECKING.

        5.  Select the **Use this Account as Default** checkbox.

        6.  Deselect the **Automatically Fill Date Received** checkbox.

2.  Process payment registrations.

    1.  Click on the **Payment Registrations** task, to open the **Register
        Customer Payments** page.

    2.  Select **Settings**, and then select **Personalize**.

        1.  Select **+ Field**.

        2.  Place the **Document No.** field on the page.

        3.  Click **Done**.

    3.  Select the line for document S20/12/0976.

        1.  Select the **Payment Made** field.

        2.  In the **Date Received** field, enter 1/24/2021.

        3.  The **Amount Received** field is automatically filled in with
            1,087.12.

    4.  Select the line for document S20/12/1576.

        1.  Select the **Payment Made** field.

        2.  In the **Date Received** field, enter 1/24/2021.

        3.  The **Amount Received** field is automatically filled in with
            2,687.68.

    5.  Select the line for document S20/12/2687.

        1.  Select the **Payment Made** field.

        2.  In the **Date Received** field, enter 1/24/2021.

        3.  In the **Amount Received** field, enter 3,000.00.

    6.  Select **Posting**, then select **Post** and then select **Post as Lump
        Payment**.
