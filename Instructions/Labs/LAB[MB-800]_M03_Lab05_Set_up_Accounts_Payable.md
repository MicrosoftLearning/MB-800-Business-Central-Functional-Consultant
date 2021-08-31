
---
lab:
    title: 'Lab: Set up Accounts Payable'
    module: 'Module 3: Configure Financials'
---

## Exercise 1: Configure the Purchases & Payables Setup

### Scenario

Concerning the processing of purchase invoices and creditmemo’s, Contoso’s
accounting manager has expressed the following requirements:

-   Posted purchase invoices and creditmemo’s are not numbered separately, but
    they follow the same numbering. This number will include the year and will
    start from 1 each year as follows:

    The first purchase document, as of January 1st 2021, will be posted with the
    number P21/0001. The next year will be P22/0001 and so on.

    These numbering should be respected in a chronological order and cannot be
    entered manually.

-   A separate g/l account 20200 is setup to record any discounts that were
    given by the vendors.

### Tasks

1.  Set up and assign number series.

2.  Complete discount posting setup.

### Steps

### Task 1

Set up and assign number series.

   1.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **Purchases & Payables Setup**, and click the  **Purchases & Payables Setup**.
   
   3.  Scroll down to the **Number Series** FastTab, and in the **Posted Invoice Nos.** field, click on the Look Up Value button
        and click **+ New**.

   3.  In the opened **No. Series List** page, fill in the following fields:

       1.  In the **Code** field, enter PINCN+

       2.  In the **Description** field, enter ‘Posted Purchase Invoices and
            Creditmemo's’.

       3.  Select the **Default Nos.** check box.

       4.  Select the **Date Order** check box.

   4.  Click the ellipse in the menubar, select **Navigate** and then select **Lines**.

   5.  In the opened **No. Series Lines** page, select **+ New**.

       1.  In the **Starting Date** field, enter 1/1/2021.

       2.  In the **Starting No.** field, enter P21/0001.

       3.  In the **Increment-by No.** field, leave the value ‘1’.
        
   6.  Close the **No. Series Lines** page.

   7.  Close the **No. Series List** page, by clicking **OK**.

   8.  The new number series PINCN+ is now automatically filled in in the
        **Posted Invoice Nos.** field, in the **Purchases & Payables Setup**
        page.

   9.  In the **Posted Credit Memo Nos**. field, enter PINCN+.

### Task 2

Complete discount posting setup.

   1.  In the **Purchases & Payables Setup** page, go to the **General**
        FastTab.

   2.  In the **Discount Posting** field, select the **All Discounts** option.

   3.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **General Posting Setup** , and click the  **General Posting Setup** link. On the page, for each possible combination of **Gen. Bus. Posting Group** and **Gen. Prod. Posting Group**, make sure  the following fields are filled in:

       1.  In the **Purch. Line Disc. Account** field, the value 20200 must be
            filled in.

       2.  In the **Purch. Inv. Disc. Account** field, the value 20200 must be
            filled in.

## Exercise 2: Create a payment journal template and batch

### Scenario

The accounting manager at Contoso would now like to use the European bank
account to make payment files.

You must set up a separate payment journal for this purpose.

### Tasks

1.  Create a general journal template.

2.  Create a general journal template batch.

### Steps

### Task 1

Create a general journal template.

   1.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **General Journal Templates** , and click the  **General Journal Templates** link.
   
   3.  In the **General Journal Templates** page, select **+ New**.

   2.  Fill in the following fields:

       1.  In the **Name** field, enter EUROP.

       2.  In the **Description** field, enter ‘Payments EUROP’.

       3.  In the **Type** field, select the **Payments** option.

       4.  In the **Bal. Account Type** field, select the **Bank Account**
            option.

       5.  In the **No. Series** field, enter GJNL-PMT.

### Task 2

Create a general journal template batch.

   1.  In the **General Journal Templates** page, make sure the EUROP journal
        is selected.

   2.  Select **More options** on the menu bar, then select **Related**, then select **Template** and then select
        **Batches**.

   3.  In the opened **General Journal Batches** page, select **+ New**.

   4.  Fill in the following fields:

       1.  In the **Name** field, enter EUROP.

       2.  In the **Description** field, enter ‘Payments EUROP’

       3.  Select the **Allow Payment Export** check box.

## Exercise 3: Create and configure vendors

### Scenario

Based on the chart of accounts, you will set up the different vendor posting
groups. With their fast growing business abroad, they want to keep track of
their accounts payables in the US (domestic) and in other EU countries (foreign)
separately. A third group will be set up to register transactions with EU
third-party alliances (intercompany) they have set up to expand their business
even further.

The DOMESTIC vendor posting group is already set up. The other vendor posting
groups will be based on this group, but with different balance accounts (20150
for foreign vendors and 20175 for intercompany vendors).

During the implementation process most of the master data for vendors was
already imported. These vendors will now have to be configured correctly by
adding the correct posting groups. First create templates based on the different
posting groups. Then apply these templates to the existing vendors.

### Tasks

1.  Set up a Vendor Posting Group.

2.  Create Configuration Templates.

3.  Configure vendors.

### Steps

### Task 1

Set up a Vendor Posting Group.

   1.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **Vendor Posting Groups** , and click the **Vendor Posting Groups** link.
   
   3.  In the **Vendor Posting Groups** page, select **+ New**.

   2.  In the **Vendor Posting Group Card** page, fill in the following fields:

       1.  In the **Code** field, fill in FOREIGN.

       2.  In the **Description** field, fill in ‘Foreign vendors’.

       3.  In the **Payables Account** field, fill in 20150.

       4.  Close the page.

   3.  In the **Vendor Posting Groups** page, select **+ New**.

   4.  In the **Vendor Posting Group Card** page, fill in the following fields:

       1.  In the **Code** field, fill in INTERCOMPANY.

       2.  In the **Description** field, fill in ‘Intercompany vendors’.

       3.  In the **Payables Account** field, fill in 20175.

       4.  Close the page.

   5.  From the **Vendor Posting Groups** page, copy the other g/l accounts
       from the DOMESTIC vendor posting group to the FOREIGN and INTERCOMPANY
        vendor posting groups using the F8 key. Copy the following fields:

       1.  Payment Disc. Debit Acc.

       2.  Payment Disc. Credit Acc.

       3.  Invoice Rounding Account

       4.  Debit Curr. Appln. Rndg. Acc.

       5.  Credit Curr. Appln. Rndg. Acc.

       6.  Debit Rounding Account
       
       7.  Credit Rounding Account

       8.  Payment Tolerance Debit Acc.

       9.  Payment Tolerance Credit Acc.

### Task 2

Create Configuration Templates.

   1.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type   **Configuration Templates** , and click the  **Configuration Templates** link.
  
   3.  In the **Configuration Templates** page, select **+ New**.

   2.  In the **Config. Template Header** page, fill in the following fields:

       1.  In the **Code** field, enter DOMESTIC
       
       2.  In the **Description** field, enter ‘Domestic vendors’

       3.  Open the assist edit button to the right of the **Table ID** field,
            select the table for vendors (ID = 23) and click **OK**.

       4.  Select the **Enabled** check box.

       5.  In the **Lines** section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

          3.  In the **Default Value** field, enter DOMESTIC

       6.  In the Lines section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Vendor Posting Group**.

          3.  In the **Default Value** field, enter DOMESTIC

       7.  Close the configuration template.

   3.  Go back to the **Configuration Templates** page, select **+ New**.

   4.  In the **Config. Template Header** page, fill in the following fields:

       1.  In the **Code** field, enter EU

       2.  In the **Description** field, enter ‘EU vendors’

       3.  Open the assist edit button to the right of the **Table ID** field,
            select the table for vendors (ID = 23) and click **OK**.

       4.  Select the **Enabled** check box.

       5.  In the **Lines** section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

          3.  In the **Default Value** field, enter EU

       6.  In the Lines section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Vendor Posting Group**.

          3.  In the **Default Value** field, enter FOREIGN

        7.  Close the configuration template.

   5.  In the **Configuration Templates** page, select **+ New**.

   6.  In the **Config. Template Header** page, fill in the following fields:

       1.  In the **Code** field, enter INTERCOMP

       2.  In the **Description** field, enter ‘Intercompany vendors’

       3.  Open the assist edit button to the right of the **Table ID** field,
            select the table for vendors (ID = 23) and click **OK**.

       4.  Select the **Enabled** check box.

       5.  In the **Lines** section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

          3.  In the **Default Value** field, enter EU

       6.  In the Lines section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Vendor Posting Group**.

          3.  In the **Default Value** field, enter INTERCOMPANY

       7.  Close the configuration template.

   7.  In the **Configuration Templates** page, select **+ New**.

   8.  In the **Config. Template Header** page, fill in the following fields:

       1.  In the **Code** field, enter EXPORT

       2.  In the **Description** field, enter ‘Export vendors’

       3.  Open the assist edit button to the right of the **Table ID** field,
            select the table for vendors (ID = 23) and click **OK**.

       4.  Select the **Enabled** check box.

       5.  In the **Lines** section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

          3.  In the **Default Value** field, enter EXPORT

       6.  In the Lines section on the page, create the following line:

          1.  In the **Type** field, enter **Field**.

          2.  In the **Field Name** field, enter **Vendor Posting Group**.

          3.  In the **Default Value** field, enter FOREIGN

       7.  Close the configuration template.

### Task 3

Configure vendors.

   1.  In the **Vendors** list page, multi-select imported vendors V9001, V9003
        and V9007.

   2.  Select **Process**, and then select **Apply Template**.
   
   3.  In the vendor templates list, select Domestic vendors, and click **OK.**

   4.  In the **Vendors** list page, multi-select imported vendors V9002, V9005
        and V9006.

   5.  Select **Process**, and then select **Apply Template**.

   6.  In the vendor templates list, select EU vendors, and click **OK.**

   7.  In the **Vendors** list page, multi-select imported vendors V9004 and
        V9008.

   8.  Select **Process**, and then select **Apply Template**.

   9.  In the vendor templates list, select Export vendors, and click **OK.**
=======
---
lab:
    title: 'Lab: Set up Accounts Payable'
    module: 'Module 3: Configure Financials'
---

## Exercise 1: Configure the Purchases & Payables Setup

### Scenario

Concerning the processing of purchase invoices and creditmemo’s, Contoso’s
accounting manager has expressed the following requirements:

-   Posted purchase invoices and creditmemo’s are not numbered separately, but
    they follow the same numbering. This number will include the year and will
    start from 1 each year as follows:

    The first purchase document, as of January 1st 2021, will be posted with the
    number P21/0001. The next year will be P22/0001 and so on.

    These numbering should be respected in a chronological order and cannot be
    entered manually.

-   A separate g/l account 20200 is setup to record any discounts that were
    given by the vendors.

### Tasks

1.  Set up and assign number series.

2.  Complete discount posting setup.

### Steps

1.  Set up and assign number series.

2.  At the top of the Business Center page, click the search icon in the black bar on the right. Then Type **Purchases & Payables Setup** and click the **Purchases & Payables Setup** link. 

3.  In the **Purchases & Payables Setup** page, go to the **Number Series** FastTab.
   **Note:** FastTabs are the bold words with aline underneath them that can be expanded. 

4.  In the **Posted Invoice Nos.** field, click on the Look Up Value button
    and click **+ New**.

5.  In the opened **No. Series List** page, fill in the following fields:

       1.  In the **Code** field, enter PINCN+

       2.  In the **Description** field, enter ‘Posted Purchase Invoices and
            Creditmemo's’.

       3.  Select the **Default Nos.** check box.

       4.  Select the **Date Order** check box.

6.  Select **Navigate** and then select **Lines**.

7.  In the opened **No. Series Lines** page, select **+ New**.

       1.  In the **Starting Date** field, enter 1/1/2021.

       2.  In the **Starting No.** field, enter P21/0001.

       3.  In the **Increment-by No.** field, leave the value ‘1’.
        
8.  Close the **No. Series Lines** page.

9.  Close the **No. Series List** page, by clicking **OK**.

10. The new number series PINCN+ is now automatically filled in in the **Posted Invoice Nos.** field, in the **Purchases & Payables Setup** page.

11. In the **Posted Credit Memo Nos**. field, enter PINCN+.

12. Complete discount posting setup.

13. In the **Purchases & Payables Setup** page, go to the **General**
    FastTab.

14. In the **Discount Posting** field, select the **All Discounts** option.

15. In the **General Posting Setup** page, for each possible combination of **Gen. Bus. Posting Group** and **Gen. Prod. Posting Group**, make sure the following fields are filled in:

       1.  In the **Purch. Line Disc. Account** field, the value 20200 must be
            filled in.

       2.  In the **Purch. Inv. Disc. Account** field, the value 20200 must be
            filled in.

## Exercise 2: Create a payment journal template and batch

### Scenario

The accounting manager at Contoso would now like to use the European bank
account to make payment files.

You must set up a separate payment journal for this purpose.

### Tasks

1.  Create a general journal template.

2.  Create a general journal template batch.

### Steps

1.  Create a general journal template.

2.  At the top of the Business Center page, in the black bar to the right, click the search icon. Then type in **General Journal Templates** and click the **General Journal Templates** link.

3.  In the **General Journal Templates** page, select **+ New**.

4.  Fill in the following fields:

       1.  In the **Name** field, enter EUROP.

       2.  In the **Description** field, enter ‘Payments EUROP’.

       3.  In the **Type** field, select the **Payments** option.

       4.  In the **Bal. Account Type** field, select the **Bank Account**
            option.

       5.  In the **No. Series** field, enter GJNL-PMT.

5.  Create a general journal template batch.

6.  In the **General Journal Templates** page, make sure the EUROP journal
    is selected.

7.  Select **Related**, then select **Template** and then select
    **Batches**.

8.  In the opened **General Journal Batches** page, select **+ New**

9.  Fill in the following fields:

       1.  In the **Name** field, enter EUROP.

       2.  In the **Description** field, enter ‘Payments EUROP’

       3.  Select the **Allow Payment Export** check box.

## Exercise 3: Create and configure vendors

### Scenario

Based on the chart of accounts, you will set up the different vendor posting
groups. With their fast growing business abroad, they want to keep track of
their accounts payables in the US (domestic) and in other EU countries (foreign)
separately. A third group will be set up to register transactions with EU
third-party alliances (intercompany) they have set up to expand their business
even further.

The DOMESTIC vendor posting group is already set up. The other vendor posting
groups will be based on this group, but with different balance accounts (20150
for foreign vendors and 20175 for intercompany vendors).

During the implementation process most of the master data for vendors was
already imported. These vendors, will now have to be configured correctly by
adding the correct posting groups. First create templates based on the different
posting groups. Then apply these templates to the existing vendors.

### Tasks

1.  Set up a Vendor Posting Group.

2.  Create Configuration Templates.

3.  Configure vendors.

### Steps

1.  Set up a Vendor Posting Group.

2.  At the top of the Business Center page, in the black bar to the right, click the search icon. Then type **Vendor Posting Groups** and click the **Vendor Posting Groups** link. 

3.  In the **Vendor Posting Groups** page, select **+ New**.

4.  In the **Vendor Posting Group Card** page, fill in the following fields:

       1.  In the **Code** field, fill in FOREIGN.

       2.  In the **Description** field, fill in ‘Foreign vendors’.

       3.  In the **Payables Account** field, fill in 20150.

       4.  Close the page.

5.  In the **Vendor Posting Groups** page, select **+ New**.

6.  In the **Vendor Posting Group Card** page, fill in the following fields:

       1.  In the **Code** field, fill in INTERCOMPANY.

       2.  In the **Description** field, fill in ‘Intercompany vendors’.

       3.  In the **Payables Account** field, fill in 20175.

       4.  Close the page.

7.  From the **Vendor Posting Groups** page, copy the other g/l accounts
   from the DOMESTIC vendor posting group to the FOREIGN and INTERCOMPANY
    vendor posting groups using F8. Copy the following fields:

       1.  Payment Disc. Debit Acc.

       2.  Payment Disc. Credit Acc.

       3.  Invoice Rouding Account

       4.  Debit Curr. Appln. Rndg. Acc.

       5.  Credit Curr. Appln. Rndg. Acc.

       6.  Debit Rounding Account
       
       7.  Credit Rounding Account

       8.  Payment Tolerance Debit Acc.

       9.  Payment Tolerance Credit Acc.

8.  Create Configuration Templates.

9.  In the **Configuration Templates** page, select **+ New**.

10. In the **Config. Template Header** page, fill in the following fields:

      1.  In the **Code** field, enter DOMESTIC

      2.  In the **Description** field, enter ‘Domestic vendors’

      3.  Open the assist edit button to the right of the **Table ID** field,
        select the table for vendors (ID = 23) and click **OK**.

      4.  Select the **Enabled** check box.

      5.  In the **Lines** section on the page, create the following line:

      6.  In the **Type** field, enter **Field**.

      7.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

      8.  In the **Default Value** field, enter DOMESTIC

      9.  In the Lines section on the page, create the following line:

      10. In the **Type** field, enter **Field**.

      11. In the **Field Name** field, enter **Vendor Posting Group**.

      12. In the **Default Value** field, enter DOMESTIC

      13. Close the configuration template.

11. In the **Configuration Templates** page, select **+ New**.

12. In the **Config. Template Header** page, fill in the following fields:

      1.  In the **Code** field, enter EU

      2.  In the **Description** field, enter ‘EU vendors’

      3.  Open the assist edit button to the right of the **Table ID** field, select the table for vendors (ID = 23) and click **OK**.

      4.  Select the **Enabled** check box.

      5.  In the **Lines** section on the page, create the following line:

      6.  In the **Type** field, enter **Field**.

      7.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

      8.  In the **Default Value** field, enter EU

      9.  In the Lines section on the page, create the following line:

      10. In the **Type** field, enter **Field**.

      11. In the **Field Name** field, enter **Vendor Posting Group**.

      12. In the **Default Value** field, enter FOREIGN

      13. Close the configuration template.

13. In the **Configuration Templates** page, select **+ New**.

14. In the **Config. Template Header** page, fill in the following fields:

      1.  In the **Code** field, enter INTERCOMP

      2.  In the **Description** field, enter ‘Intercompany vendors’

      3.  Open the assist edit button to the right of the **Table ID** field, select the table for vendors (ID = 23) and click **OK**.

      4.  Select the **Enabled** check box.

      5.  In the **Lines** section on the page, create the following line:

      6.  In the **Type** field, enter **Field**.

      7.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

      8.  In the **Default Value** field, enter EU

      9.  In the Lines section on the page, create the following line:

      10. In the **Type** field, enter **Field**.

      11. In the **Field Name** field, enter **Vendor Posting Group**.

      12. In the **Default Value** field, enter INTERCOMPANY

      13. Close the configuration template.

15. In the **Configuration Templates** page, select **+ New**.

16. In the **Config. Template Header** page, fill in the following fields:

      1.  In the **Code** field, enter EXPORT

      2.  In the **Description** field, enter ‘Export vendors’

      3.  Open the assist edit button to the right of the **Table ID** field, select the table for vendors (ID = 23) and click **OK**.

      4.  Select the **Enabled** check box.

      5.  In the **Lines** section on the page, create the following line:

      6.  In the **Type** field, enter **Field**.

      7.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

      8.  In the **Default Value** field, enter EXPORT

      9.  In the Lines section on the page, create the following line:

      10. In the **Type** field, enter **Field**.

      11. In the **Field Name** field, enter **Vendor Posting Group**.

      12. In the **Default Value** field, enter FOREIGN

      13. Close the configuration template.

17. Configure vendors.

18. In the **Vendors** list page, multi-select imported vendors V9001, V9003 and V9007.

19. Select **Process**, and then select **Apply Template**.

20. In the vendor templates list, select Domestic vendors, and click **OK**.

21. In the **Vendors** list page, multi-select imported vendors V9002, V9005 and V9006.

22. Select **Process**, and then select **Apply Template**.

23. In the vendor templates list, select EU vendors, and click **OK.**

24. In the **Vendors** list page, multi-select imported vendors V9004 and V9008.

25. Select **Process**, and then select **Apply Template**.

26. In the vendor templates list, select Export vendors, and click **OK.**
