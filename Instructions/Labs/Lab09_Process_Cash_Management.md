Exercise 9 : Process Cash Management
====================================

Task 1: Create and post journal entries
---------------------------------------

### Scenario

As the functional consultant you have prepared a configuration package for the
import of the opening balance.

The excel file contains all journal lines for all balance sheet accounts and is
prepared in the OPENING general journal, with the BALANCE journal batch,
containing dimension information.

The accounting manager at Contoso has provided you with the following opening
balance to be posted on December 28th, 2022.

You will perform

1.  Prepare the journal for the G/L opening balance.

2.  Create and export a configuration package including dimension information.

3.  Prepare data in excel.

4.  Import and apply the configuration package.

5.  Post the general journal.

### Steps

1.  Prepare the journal for the G/L opening balance.

    1.  First make sure your work date is set to **Today**.

    2.  Select the Search icon in the top-right corner of the page,
        enter `General Journals` and then choose the related link.

    3.  On the **General Journal Template List** page, select the **OPENING** journal.

    4.  Open the assist edit(…) button to the right of the **Batch Name** field.

        1.  Select the **BALANCE** journal batch.

        2.  Click **OK**.

    5.  Select **Actions**, then select **Opening Balance**, then select
        **Prepare journal** and then select **G/L Accounts Opening balance**.

    6.  Click **OK**.

    7.  The journal lines are automatically filled in for all balance accounts.

2.  Create and export a configuration package including dimension information.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Configuration Packages` and then choose the related link.

    2.  In the **Configuration Packages** page, click **+ New** to create a new
        configuration package.

    3.  In the **Code** field, enter **OPENING**.

    4.  In the **Package Name** field, enter **Opening Balances**.

    5.  On the **Tables** section of the Config. Package Card, enter a new line
        as follows.

    6.  Open the assist edit button to the right of the **Table ID** field.

    7.  In the window that opens, select the **Gen. Journal Line** table, and
        click **OK**.

    8.  Then press ENTER or TAB.

    9.  Make sure the general journal line table line is selected.

    10. Select the **Dimensions as Columns** checkbox.

    11. Select the **Delete Table Records Before Processing** checkbox.

    12. Select **Table** and then **Fields**.

    13. Click on **No.**

    14. Click on **Fields** again.

    15. On the field list page, first select **Clear Included**, to deselect the
        **Include Field** checkbox for all the fields.

    16. Then select the **Include Field** checkbox for the following fields:

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

    17. The **Validate Field** checkbox is automatically selected.

    18. Click **Close**.

    19. Select **Export to Excel**.

    20. Click **Yes** to export the configuration package.

3.  Prepare data in excel.

    1.  Open the exported excel file from the download folder.

    2.  Keep only the first 2 lines on the exported to Excel and delete all
        other, so that you can start from a blank Excel template.

    3.  **Save** the excel file.

4.  Import and apply the configuration package.

    1.  In the **Configuration Packages** page, select the new configuration
        package for opening balances and select **Manage** and then **Edit**.

    2.  In the **Config. Package Card** page, select **Import from Excel**.

    3.  Click on **Click here to browse** and select the excel file.

    4.  Click **Open**

    5.  In the preview page, select **Import**.

    6.  In the **Config. Package Card** page, select **Apply Package**.

    7.  Click **Yes**.

    8.  Click **OK**.

5.  Post the general journal.

    1.  Select the Search icon in the top-right corner of the page,
        enter `General Journals` and then choose the related link .

    2.  Click on **OPENING.**

    3.  Select the first line and enter the information as provided below.

        1.  Enter **C03** in the **Document No.** field

        2.  Enter **10100** in the **Account No.** field.

        3.  Enter **400.00** in the **Amount** field.

        4.  Enter **10200** in the **Bal. Account No.** field

    4.  Select the second line and enter the information provided below.

        1.  Enter **C04** in the **Document No.** field

        2.  Enter **10100** in the **Account No.** field.

        3.  Enter **400.00** in the **Amount** field.

        4.  Enter **10200** in the **Bal. Account No.** field

    5.  In the search area, enter General Ledger Setup and make sure the **Allow
        Posting From** field, is set to **Today**. Close the page.

    6.  Go back to **General Journal** page and then select **Post**.

    7.  Click **Yes**.

    8.  Click **OK**.

Task 2: Create and post journal entries
---------------------------------------

### Scenario

The accounting manager at Contoso also provided you with the open customer and
vendor ledger entries.

You receive the configuration package, that you can import into the correct
general journals, review, and post.

*(Remark: if you do not have the configuration package for this lab, you can use
the configuration package from Task 1 and use the excel sheet to import these
opening ledger entries)*

You will perform

1.  Import and apply a predefined package containing historical data (customer
    and vendor open entries).

2.  Post the general journal.

### Steps

1.  Import and apply a predefined package containing historical data (customer
    and vendor open entries).

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Configuration Packages**, and then choose the related link.

    2.  On the **Configuration Packages** page, select the **OPENING** package
        and then select **Import Package**.

    3.  Click on **Click here to browse.**

    4.  Select the rapidstart package.

    5.  In the **Config. Package Card** page, select **Package** and then
        **Apply Package**.

    6.  Click **Yes**.

    7.  Click **OK**.

2.  Post the general journal.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **General Journals**, and then choose the related link.

    2.  On the **General Journals** list page, select the **OPENING** journal.

    3.  Open the assist edit button to the right of the **Batch Name** field.

        1.  Select the **CUST** journal batch.

        2.  Click **OK**.

    4.  Select the first line and fill in the following details.

        1.  Update the **Posting Date** field of all the lines

        2.  Enter **D01** in the **Document No.** field

        3.  Enter **10100** in the **Account No.** field

        4.  Enter **400.00** in the **Amount** field

    5.  Repeat the above for line number 2, 3 and 4

    6.  Enter **10200** in the **Balance Account No.** field of all the lines

    7.  Select **Post**.

    8.  Click **Yes**.

    9.  Click **OK**.

    10. Close the General Journals Page.

    11. Enter **General Journals** in the search and select the related link.

    12. Open the assist edit button to the right of the **Batch Name** field.

        1.  Select the **VEND** journal batch.

        2.  Click **OK**.

    13. Update the Posting Date field of all the lines.

    14. Select **Home**, and then select **Post**.

    15. Click **Yes**.

    16. Click **OK**.

Task 3: Process vendor payments
-------------------------------

### Scenario

At the end of each month all euro payments are transferred from the EUROP bank
account to the European vendors, using an electronic SEPA file. Each time a
payment is performed a new payment journal batch is created.

Vendor First Up Consultants has recently changed their bank account and has
asked you to make sure the next euro payment will be done on that Belgian
account. They also request to be paid for all invoices as a single payment.

The bank account details: SNS - IBAN: BE67 2900 0461 4187 - SWIFT Code: BBRUBEBB

The first payment to this vendor V9005 will be performed on January 31st, 2023,
using the EUROP payment journal, with a new batch PAY1.

You will perform

1.  Create a vendor bank account.

2.  Suggest vendor payments.

3.  Process payment journals.

### Steps

1.  Create a vendor bank account.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Vendors` and then choose the related link.

    2.  On the **Vendors** list page, select vendor **Graphic Design
        Institute.**

    3.  Select **Manage** and then select **Edit**.

    4.  On the **Vendor** card, go to the **Payments** Fast Tab.

    5.  In the **Preferred Bank Account Code** field, click on the Look Up Value
        button and click **+ New**.

    6.  On the opened **Vendor bank account** card, fill in the following
        fields:

        1.  On the **General** FastTab, fill in the following fields:

            1.  In the **Code** field, enter **SNS**.

            2.  In the **Name** field, enter **Graphic Design Institute**.

            3.  In the **Country/Region Code** field, enter **BE**.

            4.  In the **Currency Code** field, enter **EUR**.

        2.  On the **Transfer** FastTab, click **Show more** and then fill in
            the following fields:

            1.  In the **SWIFT Code** field, enter **BBRUBEBB**.

            2.  In the **IBAN** field, enter **BE67290004614187**.

            3.  Select the **Use for Electronic Payments** checkbox.

        3.  Click **OK**.

    7.  The new **Vendor bank account** is automatically filled in in the
        **Preferred Bank Account Code** field on the vendor card.

2.  Suggest vendor payments.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Payment journals` and then choose the related link.

    2.  Open the assist edit button to the right of the **Batch Name** field.

    3.  On the opened **General Journal Batches** page, click **+ New** and fill
        in the following fields:

        1.  In the **Name** field, enter **PAY1**.

        2.  In the **Description** field, enter **Payment January 2023**.

        3.  In the **Bal. Account Type** field, enter **Bank Account**.

        4.  In the **Bal. Account No.** field, enter **EUROP**. (If you do not
            find the value, create a new value with **EUROP**)

        5.  In the **No. Series** field, the value **GJNL-PMT** is automatically
            filled in.

        6.  Click **OK**.

    4.  The new batch **PAY1**, is automatically filled in in the **Batch Name**
        field on the payment journal.

    5.  Select **Prepare**, and then select **Suggest Vendor Payments**.

    6.  On the **Options** FastTab, fill in the following fields:

        1.  In the **Last Payment Date** field, enter **1/31/2023**.

        2.  Leave the **Check Other Journal Batches** checkbox selected.

        3.  Select the **Summarize per Vendor** checkbox.

        4.  On the **Filter:Vendor** FastTab, in the **No**. filter, enter
            **20000**.

        5.  Click **OK** to perform the batch job and automatically fill in the
            lines in the payment journal.

g. In the second line, fill in the details. Enter **V9005** in the **Account
No.** field. Enter **4000.00** in the **Amount** field

h. Process payment journals. Select **Bank**, and then select **Export**.

1.  Select **Home**, and then select **Post**.

2.  Click **Yes**.

3.  Click **OK**.

Task 4: Process customer payments
---------------------------------

### Scenario

On January 24th, 2023, Contoso receives payment from customer C00010
Spotsmeyer’s Furnishings on their CHECKINGS bank account.

This payment is for all open invoices from the previous month:

-   S-ORD101009 - \$ 5,828.00

-   Opening balance - \$ 5,345.16

-   Opening balance - \$ 5,345.16

You need to process this payment using the Payment Registration by applying the
invoices.

You will perform

1.  Review payment registration setup.

2.  Process payment registrations.

### Steps

1.  Review payment registration setup.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Payment Registration Setup` and then choose the related link.

    2.  On the **Payment Registration Setup** page, make sure following fields
        are entered.

        1.  In the **Journal Template Name** field, enter **CASHRCPT**.

        2.  In the **Journal Batch Name** field, enter **GENERAL**.

        3.  In the **Balancing Account Type** field, enter **Bank Account**.

        4.  In the **Balancing Account** field, enter **CHECKING**.

        5.  Select the **Use this Account as Default** checkbox.

        6.  Deselect the **Automatically Fill Date Received** checkbox.

        7.  Click **OK**.

2.  Process payment registrations.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Payment Registrations`.

    2.  Click on the **Payment Registrations** task, to open the **Register
        Customer Payments** page.

    3.  Select the line for document **S-ORD101009**.

        1.  Select the **Payment Made** field.

        2.  In the **Date Received** field, enter **1/24/2023**.

        3.  The **Amount Received** field is automatically filled in with
            **5,828.00**.

    4.  Select the line for document **Opening balance**.

        1.  Select the **Payment Made** field.

        2.  In the **Date Received** field, enter **1/24/2023**.

        3.  The **Amount Received** field is automatically filled in with
            **5,345.16**.

    5.  Select the line for document **Opening balance**.

        1.  Select the **Payment Made** field.

        2.  In the **Date Received** field, enter **1/24/2023**.

        3.  In the **Amount Received** field, enter **5,345.16**.

    6.  Select the dropdown of **Post Payments** and then select **Post as Lump
        Payment**.

    7.  Click **Yes** to post all the three payments.
