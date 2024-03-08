Exercise 10: Set Up Accounts Payable
====================================

Task 1: Configure the Purchases & Payables Setup
------------------------------------------------

### Scenario

Concerning the processing of purchase invoices and credit memos, Contoso’s
accounting manager has expressed the following requirements:

-   Posted purchase invoices and credit memos are not numbered separately, but
    they follow the same numbering. This number will include the year and will
    start from 1 each year as follows:

    The first purchase document, as of January 1st, 2022, will be posted with
    the number P22/0001. The next year will be P23/0001 and so on.

    These numbering should be respected in a chronological order and cannot be
    entered manually.

-   A separate g/l account 20200 is setup to record any discounts that were
    given by the vendors.

You will perform

1.  Set up and assign number series.

2.  Complete discount posting setup.

### Steps

1.  Set up and assign number series.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Purchases & Payables Setup**, and then choose the related link.

    2.  In the **Purchases & Payables Setup** page, go to the **Number Series**
        FastTab.

    3.  In the **Posted Invoice Nos.** field, click on the Look Up Value button
        and click **+ New.**

    4.  In the opened **No. Series List** page, fill in the following fields:

        1.  In the **Code** field, enter **PINCN+**

        2.  In the **Description** field, enter **Posted Purchase Invoices and
            Credit memos**.

        3.  Select the **Default Nos.** check box.

        4.  Select the **Date Order** check box.

    5.  Click the ellipses (…), select **Navigate** and then select **Lines**.

    6.  In the opened **No. Series Lines** page, select **+ New**.

        1.  In the **Starting Date** field, enter **1/1/2023**.

        2.  In the **Starting No.** field, enter **P22/0001**.

        3.  In the **Increment-by No.** field, leave the value **1**.

    7.  Close the **No. Series Lines** page.

    8.  Close the **No. Series List** page, by clicking **OK**.

    9.  The new number series PINCN+ is now automatically filled in in the
        **Posted Invoice Nos.** field, in the **Purchases & Payables Setup**
        page.

    10. In the **Posted Credit Memo Nos**. field, enter **PINCN+**.

2.  Complete discount posting setup.

    1.  In the **Purchases & Payables Setup** page, go to the **General**
        FastTab.

    2.  In the **Discount Posting** field, select the **All Discounts** option.

    3.  Select the search for page icon in the top-right corner of the page,
        enter **General Posting Setup**, and then choose the related link.

    4.  In the **General Posting Setup** page, for each possible combination of
        **Gen. Bus. Posting Group** and **Gen. Prod. Posting Group**, make sure
        the following fields are filled in:

        1.  In the **Purch. Line Disc. Account** field, the value **20200** must
            be filled in.

        2.  In the **Purch. Inv. Disc. Account** field, the value **20200** must
            be filled in.

Note – If you do not find the value – Please proceed with creating a new.

Task 2: Create a payment journal template and batch
---------------------------------------------------

### Scenario

The accounting manager at Contoso would now like to use the European bank
account to make payment files.

You must set up a separate payment journal for this purpose.

You will perform

1.  Create a general journal template.

2.  Create a general journal template batch.

### Steps

1.  Create a general journal template.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **General Journal Templates**, and then choose the related link.

    2.  In the **General Journal Templates** page, select **+ New**.

    3.  Fill in the following fields:

        1.  In the **Name** field, enter **EUROP**.

        2.  In the **Description** field, enter **Payments EUROP**.

        3.  In the **Type** field, select the **Payments** option.

        4.  In the **Bal. Account Type** field, select the **Bank Account**
            option.

        5.  In the **No. Series** field, enter **GJNL-PMT**.

2.  Create a general journal template batch.

    1.  In the **General Journal Templates** page, make sure the **EUROP**
        journal is selected.

    2.  Select **Batches**.

    3.  In the opened **General Journal Batches** page, select **+ New.**

    4.  Fill in the following fields:

        1.  In the **Name** field, enter **EUROP**.

        2.  In the **Description** field, enter **Payments EUROP**

        3.  Select the **Allow Payment Export** check box.

Task 3: Create and configure vendors
------------------------------------

### Scenario

Based on the chart of accounts, you will set up the different vendor posting
groups. With their fast-growing business abroad, they want to keep track of
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

You will perform

1.  Set up a Vendor Posting Group.

2.  Create Vendor Templates.

3.  Configure vendors.

### Steps

1.  Set up a Vendor Posting Group.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Vendor Posting Groups**, and then choose the related link.

    2.  In the **Vendor Posting Groups** page, select **+ New**.

    3.  In the **Vendor Posting Group Card** page, fill in the following fields:

        1.  In the **Code** field, fill in **FOREIGN**.

        2.  In the **Description** field, fill in **Foreign vendors**.

        3.  In the **Payables Account** field, fill in **20150**.

        4.  Close the page.

    4.  In the **Vendor Posting Groups** page, select **+ New**.

    5.  In the **Vendor Posting Group Card** page, fill in the following fields:

        1.  In the **Code** field, fill in **INTERCOMPANY**.

        2.  In the **Description** field, fill in **Intercompany vendors**.

        3.  In the **Payables Account** field, fill in **20175**.

        4.  Close the page.

    6.  From the **Vendor Posting Groups** page, copy the other g/l accounts
        from the **DOMESTIC** vendor posting group to the **FOREIGN** and
        **INTERCOMPANY** vendor posting groups. Copy the following fields:

        1.  Payment Disc. Debit Acc.

        2.  Payment Disc. Credit Acc.

        3.  Invoice Rouding Account

        4.  Debit Curr. Appln. Rndg. Acc.

        5.  Credit Curr. Appln. Rndg. Acc.

        6.  Debit Rounding Account

        7.  Credit Rounding Account

        8.  Payment Tolerance Debit Acc.

        9.  Payment Tolerance Credit Acc.

2.  Create Vendor Templates.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Vendor Templates**, and then choose the related link.

    2.  In the **Vendor Templates** page, select **+ New**.

    3.  In the opened **Vendor Template** page, fill in the following fields:

        1.  In the **Code** field, enter **DOMESTIC**

        2.  In the **Description** field, enter **Domestic vendors**

        3.  Then go to the **Invoicing** FastTab and fill in the following
            fields:

3.  In the **Gen. Bus. Posting Group** field, enter **DOMESTIC**.

4.  In the **Vendor Posting Group** field, enter **DOMESTIC**.

    1.  Close the vendor template.

    2.  In the **Vendor Templates** page, select **+ New**.

    3.  In the opened vendor template:

5.  Go to the **General** FastTab and fill in the following fields:

    1.  In the **Code** field, enter **EU**

    2.  In the **Description** field, enter **EU vendors**

6.  Then go to the **Invoicing** FastTab and fill in the following fields:

    1.  In the **Gen. Bus. Posting Group** field, enter **EU**.

    2.  In the **Vendor Posting Group** field, enter **FOREIGN**.

7.  Close the vendor template.

    1.  In the **Vendor Templates** page, select **+ New**.

    2.  In the opened vendor template:

    3.  Go to the **General** FastTab and fill in the following fields:

        1.  In the **Code** field, enter **INTERCOMP**

        2.  In the **Description** field, enter **Intercompany vendors**

    4.  Then go to the **Invoicing** FastTab and fill in the following fields:

        1.  In the **Gen. Bus. Posting Group** field, enter **EU**.

        2.  In the **Vendor Posting Group** field, enter **INTERCOMP**.

    5.  Close the vendor template.

    6.  In the **Vendor Templates** page, select **+ New**.

    7.  In the opened vendor template:

8.  Go to the **General** FastTab and fill in the following fields:

    1.  In the **Code** field, enter **EXPORT**

    2.  In the **Description** field, enter **Export vendors**

9.  Then go to the **Invoicing** FastTab and fill in the following fields:

    1.  In the **Gen. Bus. Posting Group** field, enter **EXPORT**.

    2.  In the **Vendor Posting Group** field, enter **FOREIGN**.

10. Close the **Vendor Template**.

11. Configure vendors.

12. Select the search for page icon in the top-right corner of the page, enter
    **Vendors**, and then choose the related link.

13. In the **Vendors** page, multi-select imported vendors **V9001**, **V9003**
    and **V9007**.

14. Select **Apply Template**.

15. In the **Vendor Templates** list, select **Domestic vendors**, and click
    **OK.**

16. Click **Yes**.

17. In the **Vendors** list page, multi-select imported vendors **V9002**,
    **V9005** and **V9006**.

18. Select **Apply Template**.

19. In the **Vendor Templates** list, select **EU vendors**, and click **OK.**

20. Click **Yes**.

21. In the **Vendors** list page, multi-select imported vendors **V9004** and
    **V9008**.

22. Select **Apply Template**.

23. In the **Vendor Templates** list, select **Export vendors**, and click
    **OK.**

24. Click **Yes**.
