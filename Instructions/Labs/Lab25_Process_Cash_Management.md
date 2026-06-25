---
lab:
  title: 'Lab 25: Process Cash Management and general journal entries'
  module: 'Perform a bank reconciliation in Dynamics 365 Business Central'
  duration: 60 minutes
  level: 300
  islab: true
---

## Exercise 25: Process Cash Management

## Task 1: Create and post journal entries

## Scenario
As the functional consultant you have prepared a configuration package for the import of the opening balance.

The excel file contains all journal lines for all balance sheet accounts and is prepared in the OPENING general journal, with the BALANCE journal batch, containing dimension information.

The accounting manager at Contoso has provided you with the following opening balance to be posted on December 31th, 2025.

You will perform

1. Prepare the journal for the G/L opening balance.
2. Update and post the general journal.

### Steps
1. Prepare the journal for the G/L opening balance.
   1. First make sure your work date is set to **Today**.
   2. Select the Search icon in the top-right corner of the page, enter General Journals and then choose the related link.
   3. On the **General Journal Template List** page, select the **OPENING** journal.
   4. Open the assist edit(…) button to the right of the **Batch Name** field.
      1. Select the **BALANCE** journal batch.
      2. Select **OK**.
   5. Select **Actions**, then select **Opening Balance**, then select **Prepare journal** and then select **G/L Accounts Opening balance**.
   6. Select **OK**.
   7. The journal lines are automatically filled in for all balance accounts.
   8. h
2. IUpdate and post the general journal.
   1. Select the Search icon in the top-right corner of the page, enter General Journals and then choose the related link .
   2. Select on **OPENING.**
   3. In Batch Name field select **BALANCE**.
   4. Set filter to Account No. <>10100 and delete all journal lines. Remove filter.
   5. Slect the first line and add the information as provided below.
      1. Enter **C03** in the **Document No.** field
      2. Enter **10100** in the **Account No.** field.
      3. Enter **400.00** in the **Amount** field.
      4. Enter **10200** in the **Bal. Account No.** field
   6. Select the second line and enter the information provided below.
      1. Enter **C04** in the **Document No.** field
      2. Enter **10100** in the **Account No.** field.
      3. Enter **400.00** in the **Amount** field.
      4. Enter **10200** in the **Bal. Account No.** field
   7. In the search area, enter **General Ledger Setup** and make sure the **Allow Posting From** field, is set to **Today or blank**. Close the page.
   8. Go back to **General Journal** page and then select **Post**.
   9. Select **Yes**.
   10. Select **OK**.

## Task 2: Create and post journal entries

## Scenario
The accounting manager at Contoso also provided you with the open customer and vendor ledger entries. You create configuration package to import open balances entries.

You receive the configuration package, that you can import into the correct general journals, review, and post.

You will perform

1. Create and export a configuration package including dimension information.
2. Import and apply a predefined package containing historical data (customer and vendor open entries).
3. Post the general journal.

### Steps
1. Create a configuration package including dimension information.
   1. Select the Search icon in the top-right corner of the page, enter Configuration Packages and then choose the related link.
   2. In the **Configuration Packages** page, select **+ New** to create a new configuration package.
   3. In the **Code** field, enter **OPENING**.
   4. In the **Package Name** field, enter **Opening Balances**.
   5. On the **Tables** section of the Config. Package Card, enter a new line as follows.
   6. Open the assist edit button to the right of the **Table ID** field.
   7. In the window that opens, select the **Gen. Journal Line** table (ID 81), and select **OK**.
   8. Then press ENTER or TAB.
   9. Make sure the general journal line table line is selected.
   10. Select the **Dimensions as Columns** checkbox.
   11. Select the **Delete Table Records Before Processing** checkbox.
   12. Select **Table** and then **Fields**.
   13. System gets a message: Some fields have two or more related tables. Do you want to check them? Select on **No.**
   14. Select on **Fields** again.
   15. On the field list page, first select **Clear Included**, to deselect the **Include Field** checkbox for all the fields.
   16. Then select the **Include Field** checkbox for the following fields:
       1. Account Type
       2. Account No.
       3. Posting Date
       4. Document Type
       5. Document No.
       6. Description
       7. Currency Code
       8. Amount
       9. Amount (LCY)
       10. Document Date
       11. External Document No.
   17. The **Validate Field** checkbox is automatically selected.
   18. Select **Close**.
2. Import and apply a predefined package containing historical data (customer and vendor open entries).
   1. Select the search for page icon in the top-right corner of the page, enter **Configuration Packages**, and then choose the related link.
   2. On the **Configuration Packages** page, select the **OPENING** package and then select **Import Package/Import from Excel**.
   3. Select on **Select here to browse.**
   4. Select the Excel file **OpenBalance Lab 8.2.xlsx**.
   5. In the **Config. Package Card** page, select **Package** and then **Apply Package**.
   6. Select **Yes**.
   7. Select **OK**.
3. Post the general journal.
   1. Select the search for page icon in the top-right corner of the page, enter **General Journals**, and then choose the related link.
   2. On the **General Journals** list page, select the **OPENING** journal.
   3. Open the assist edit button to the right of the **Batch Name** field.
      1. Select the **CUST** journal batch.
      2. Select **OK**.
   4. Select Post -> Preview Posting
   5. Check for any errors and correct them
   6. Close the window
   7. Select **Post**
   8. Select **Yes**
   9. Select **OK**
   10. Close the General Journals Page.
   11. Enter **General Journals** in the search and select the related link.
   12. On the **General Journals** list page, select the **OPENING** journal.
   13. Open the assist edit button to the right of the **Batch Name** field.
       1. Select the **VEND** journal batch.
       2. Select **OK**.
   14. Select Post -> Preview Posting
   15. Check for any errors and correct them
   16. Close the window
   17. Select **Post**
   18. Select **Yes**
   19. Select **OK**
   20. Close the General Journals Page.
   21. Select **Home**, and then select **Post**.
   22. Select **Yes**.
   23. Select **OK**.

## Task 3: Process vendor payments

## Scenario
At the end of each month all euro payments are transferred from the EUROP bank account to the European vendors, using an electronic SEPA file. Each time a payment is performed a new payment journal batch is created.

Vendor First Up Consultants has recently changed their bank account and has asked you to make sure the next euro payment will be done on that Belgian account. They also request to be paid for all invoices as a single payment.

The bank account details: SNS - IBAN: BE67 2900 0461 4187 - SWIFT Code: BBRUBEBB

The first payment to this vendor V9005 will be performed on January 31st, 2026, using the EUROP payment journal, with a new batch PAY1.

You will perform

1. Create a vendor bank account.
2. Suggest vendor payments.
3. Process payment journals.

### Steps
1. Create a vendor bank account.
   1. Select the Search icon in the top-right corner of the page, enter Vendors and then choose the related link.
   2. On the **Vendors** list page, select vendor **Graphic Design Institute.**
   3. On the **Vendor** card, go to the **Payments** Fast Tab.
   4. In the Payment Method Code field, select BANK.
   5. In the **Preferred Bank Account Code** field, select on the Look Up Value button and select **+ New**.
   6. On the opened **Vendor bank account** card, fill in the following fields:
      1. On the **General** FastTab, fill in the following fields:
         1. In the **Code** field, enter **SNS**.
         2. In the **Name** field, enter **Graphic Design Institute**.
         3. In the **Country/Region Code** field, enter **BE**.
         4. In the **Currency Code** field, enter **EUR**.
      2. On the **Transfer** FastTab, select **Show more** and then fill in the following fields:
         1. In the **SWIFT Code** field, enter **BBRUBEBB**.
         2. In the **IBAN** field, enter **BE67290004614187**.
         3. Select the **Use for Electronic Payments** checkbox.
      3. Select **OK**.
   7. The new **Vendor bank account** is automatically filled in in the **Preferred Bank Account Code** field on the vendor card.
2. Suggest vendor payments.
   1. Select the Search icon in the top-right corner of the page, enter Payment journals and then choose the related link.
   2. On the opened **General Journal Batches** page, select **+ New** and fill in the following fields:
      1. In the **Name** field, enter **PAY1**.
      2. In the **Description** field, enter **Payment January 2026**.
      3. In the **Bal. Account Type** field, enter **Bank Account**.
      4. In the **Bal. Account No.** field, enter **EUROP**. (If you do not find the value, create a new value with **EUROP**)
      5. In the **No. Series** field, the value **GJNL-PMT** is automatically filled in.
      6. Select **OK**.
   3. The new batch **PAY1**, is automatically filled in in the **Batch Name** field on the payment journal.
   4. Select **Prepare**, and then select **Suggest Vendor Payments**.
   5. On the **Options** FastTab, fill in the following fields:
      1. In the **Last Payment Date** field, enter **1/31/2026**.
      2. In the Posting Date field, leave the current date.
      3. Leave the **Check Other Journal Batches** checkbox selected.
      4. Select the **Summarize per Vendor** checkbox.
      5. On the **Filter:Vendor** FastTab, in the **No**. filter, enter 3**0000**.
      6. Select **OK** to perform the batch job and automatically fill in the lines in the payment journal.

g. In the second line, fill in the details. Enter30000 in the **Account No.** field. Enter **4000.00** in the **Amount** field

h. Process payment journals. Select **Bank**, and then select **Export**.

1. Select **Home**, and then select **Post**.
2. Select **Yes**.
3. Select **OK**.

## Task 4: Process customer payments

## Scenario
On January 24th, 2026 , Contoso receives payment from customer 30000 Trey Research on their CHECKINGS bank account.

This payment is for all open invoices from the previous month:

* Opening balance - $ 5,345.16
* Opening balance - $ 5,345.16

You need to process this payment using the Payment Registration by applying the invoices.

You will perform

1. Review payment registration setup.
2. Process payment registrations.

[Steps

1. Review payment registration setup.
   1. Select the Search icon in the top-right corner of the page, enter Payment Registration Setup and then choose the related link.
   2. On the **Payment Registration Setup** page, make sure following fields are entered.
      1. In the **Journal Template Name** field, enter **CASHRCPT**.
      2. In the **Journal Batch Name** field, enter **GENERAL**.
      3. In the **Balancing Account Type** field, enter **Bank Account**.
      4. In the **Balancing Account** field, enter **CHECKING**.

[NOTE]if you don’t have CHECKING bank account, you must first create it.

Choose +New

In the No. field enter CHECKING.

In the Name enter CHECKINGS bank account.

On the Posting section in the Bank Acc. Posting group choose CHECKING.

Select OK.

* + 1. Select the **Use this Account as Default** checkbox.
    2. Deselect the **Automatically Fill Date Received** checkbox.
    3. Select **OK**.

1. Process payment registrations.
   1. Select the Search icon in the top-right corner of the page, enter **Register Customer Payments**.
   2. Select the line for document **Opening balance** for 20000 Trey Research customer
      1. Select the **Payment Made** field.
      2. In the **Date Received** field, enter **1/24/2026**.
      3. The **Amount Received** field is automatically filled in with **5,345.16**.
   3. Select the line for document **Opening balance**.
      1. Select the **Payment Made** field.
      2. In the **Date Received** field, enter **1/24/2026**.
      3. In the **Amount Received** field, enter **5,345.16**.
   4. Select the **Post Payments** dropdown, and then select **Post Payments**.
   5. Select **Yes** to post all the payments.