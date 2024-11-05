Exercise 11: Set Up Accounts Receivable
=======================================

Task 1: Configure the Sales & Receivables Setup
-----------------------------------------------

### Scenario

Concerning the processing of sales transactions, Contoso’s account manager has
expressed the following requirements:

-   Web shop customers will be numbered separately from other customers. Regular
    customers are numbered C00010 and incremented by 10. Web shop customers are
    numbered CWEB00010 and incremented by 10.

    *(Remark: The number series for regular customers is already created (CUST)
    and assigned in the Sales & Receivables Setup)*

-   Posted sales invoices are numbered based on the year and month in which they
    are posted. The first sales invoice, as of January 1st, 2022, will be posted
    with the number S22/01/0001. The next month will be S22/02/0001 and so on.

-   A separate g/l account 40300 is setup to record invoice discounts only that
    were given to the customer. Line discounts are also given but considered as
    part of the net sales price and thus not posted separately from the normal
    sales account.

-   Contoso works with a credit insurer, who provides credit limits for each
    customer. When this limit is reached, salespeople have to communicate with
    the finance department before going ahead with the sale.

You will perform

1.  Set up and assign number series

2.  Complete discount posting setup

3.  Activate credit limit warning

### Steps

1.  Set up and assign number series.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Sales & Receivables Setup`, and then choose the related link.

    2.  In the **Sales & Receivables Setup** page, go to the **Number Series**
        FastTab.

    3.  In the **Customer Nos.** field, the value CUST is already filled in. Click on
        the Look Up Value button and select **+ New**.

    4.  In the opened **No. Series** page, fill in the following fields:

        1.  In the **Code** field, enter **CUST WEB**

        2.  In the **Description** field, enter **Customers Web Shop**.

        3.  Select the **Default Nos.** check box.

    5.  Click on the ellipses (…) in the top ribbon
     and then select **Lines**.

    6.  In the opened **No. Series Lines** page, select **+ New**.

        1.  Leave the **Starting Date** field blank.

        2.  In the **Starting No.** field, enter **CWEB0001**.

        3.  In the **Increment-by No.** field, enter the value **10**.

    7.  Close the **No. Series Lines** page.

    8.  In the opened **No. Series** page, select the number series
        **CUST**.

    9.  Click the ellipses (…) and then select
        **Relationships**.

    10. In the **No. Series Relationships** page, select **+ New**.

    11. In the **Series Code** field, enter **CUST WEB.**

    12. Close the **No. Series Relationships** page.

    13. Close the **No. Series** page by clicking **OK**.

    14. You are now back in the **Sales & Receivables Setup** page, on the
        **Number Series** FastTab.

    15. In the **Posted Invoice Nos.** field, the value **S-INV+** is already
        filled in. Click on the Look Up Value button and then click **Select
        from full list.**

    16. In the opened **No. Series** page, the number series **S-INV+** is
        automatically selected.

    17. Select **Lines**.

    18. In the opened **No. Series Lines** page, select **+ New**.

        1.  In the **Starting Date** field, enter **1/1/2022**.

        2.  In the **Starting No.** field, enter **S22/01/0001**.

        3.  In the **Increment-by No.** field, leave the value **1**.

    19. In the opened **No. Series Lines** page, select **+ New**.

        1.  In the **Starting Date** field, enter **2/1/2022**.

        2.  In the **Starting No.** field, enter **S22/02/0001**.

        3.  In the **Increment-by No.** field, leave the value **1**.

    20. Close the **No. Series Lines** page.

    21. Close the **No. Series** page by clicking **OK**.

    22. The number series **S-INV+** remains filled in in the **Posted Invoice
        Nos.** field, in the **Sales & Receivables Setup** page.

2.  Complete discount posting setup.

    1.  In the **Sales & Receivables Setup** page, go to the **General**
        FastTab.

    2.  In the **Discount Posting** field, select the **Invoice Discounts**
        option.

    3.  Select the search for page icon in the top-right corner of the page,
        enter **General Posting Setup**, and then choose the related link.

    4.  In the **General Posting Setup** page, for each possible combination of
        **Gen. Bus. Posting Group** and **Gen. Prod. Posting Group**, make sure
        the **Sales Inv. Disc. Account** field is filled in with the value
        **40301**. If you are unable to see, please proceed with the creating a
        new.

3.  Activate credit limit warning

    1.  In the **Sales & Receivables Setup** page, go to the **General**
        FastTab.

    2.  In the **Credit Warnings** field, select the **Credit Limit** option.

Task 2: Create and configure customers
--------------------------------------

### Scenario

Based on the chart of accounts, you will set up the different customer posting
groups. With their fast-growing business abroad, they want to keep track of
their accounts receivables in the US (domestic) and in other EU countries
(foreign) separately. A third group will be set up to register transactions with
EU third-party alliances (intercompany) they have set up to expand their
business even further.

The DOMESTIC customer posting group is already set up. The other customer
posting groups will be based on this group, but with different balance accounts
(10450 for foreign customers and 10475 for intercompany customers).

A generic EU web shop customer will be created for all end-user customers that
prefer not to create a Contoso customer account. Make sure to fill in the
correct posting groups and that the following requirements are met:

-   All sales documents will be mailed as a pdf-file to the customer’s default
    Email-address and the document will also be stored as a pdf-file.

-   End user customers need to pay sales invoices before delivery using a credit
    card service. Credit card payments will be posted to the g/l account 20500
    when processing the sales invoice.

-   This fictitious customer is considered to always be part of the small
    business customer group.

You need to create this customer manually.

*Remark: before starting this exercise, first disable the existing configuration
templates for customers: CUST000001 & CUST000002*

You will perform

1.  Set up a Customer Posting Group.

2.  Create and configure a new customer

### Steps

1.  Set up a Customer Posting Group

    1.  Select the Search icon in the top-right corner of the page,
        enter `Customer Posting Groups`, and then choose the related link.

    2.  In the **Customer Posting Groups** page, select **+ New**.

    3.  In the **Customer Posting Group Card** page, fill in the following
        fields:

        1.  In the **Code** field, fill in **FOREIGN**.

        2.  In the **Description** field, fill in **Foreign customers**.

        3.  In the **Receivables Account** field, fill in **10450**.

        4.  Close the page.

    4.  In the **Customer Posting Groups** page, select **+ New**.

    5.  In the **Customer Posting Group Card** page, fill in the following
        fields:

        1.  In the **Code** field, fill in **INTERCOMPANY**.

        2.  In the **Description** field, fill in **Intercompany customers**.

        3.  In the **Receivables Account** field fill in **10475**.

        4.  Close the page.

    6.  From the **Customer Posting Groups** page, copy the other g/l accounts
        from the DOMESTIC customer posting group to the **FOREIGN** and
        **INTERCOMPANY** customer posting groups using F8. Copy the following
        fields:

        1.  Payment Disc. Debit Acc.

        2.  Payment Disc. Credit Acc.

        3.  Interest Account

        4.  Additional Fee Account

        5.  Invoice Rouding Account

        6.  Debit Curr. Appln. Rndg. Acc.

        7.  Credit Curr. Appln. Rndg. Acc.

        8.  Debit Rounding Account

        9.  Credit Rounding Account

        10. Payment Tolerance Debit Acc.

        11. Payment Tolerance Credit Acc.

2.  Create and configure a new customer.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Customers`, and then choose the related link.

    2.  In the **Customers** page, select **+ New**.

    3.  Select the **CUSTOMER COMPANY** template and then click **OK**.

    4.  Go to the **General** FastTab.

    5.  Open the assist edit button to the right of the **No.** field.

    6.  In the window that opens, select the number series for web shop
        customers **CUST WEB** and click **OK**.

    7.  Click **Yes**.

    8.  In the **Name** field, enter **Generic EU web shop**.

    9.  Click **Show more**.

    10. In the **Document Sending Profile** field, click on the Look Up Value
        button and click **+ New**.

    11. In the opened **Document Sending Profile** card page, fill in the
        following fields:

        1.  In the **Code** field, enter **MAIL&PDF**.

        2.  In the **Description** field, enter **Mail & PDF**.

        3.  In the **Email** field, select the **Yes (Use Default Settings)**
            option.

        4.  The **Email Attachment** field is automatically set to the **PDF**
            option.

        5.  In the **Disk** field, select the **PDF** option.

        6.  Click **OK**.

    12. The new code is now automatically filled  in the **Document Sending
        Profile** field on the customer card.

    13. Go to the **Invoicing** FastTab.

    14. In the **Gen. Bus. Posting Group** field, enter **EU**.

    15. In the **Customer Posting Group**, enter **FOREIGN.**

    16. Go to the **Payments** FastTab.

    17. In the **Payment Terms Code** field, click on the Look Up Value button
        and click **+ New**.

    18. In the opened **Payment Terms** page, select **+ New** and fill in the
        following fields:

        1.  In the **Code** field, enter **0 DAYS**.

        2.  In the **Due Date Calculation** field, enter **0D**.

        3.  In the **Description** field, enter **Pay before delivery**.

        4.  Click **OK**.

    19. The new code is now automatically filled in in the **Payment Terms
        Code** field on the customer card.

    20. On the **Payments** FastTab, click **Show more**.

    21. In the **Payment Method Code** field, click on the Look Up Value button
        and click **+ New**.

    22. In the opened **Payment Methods** page, select **+ New** and fill in the
        following fields:

        1.  In the **Code** field, enter **CREDITCARD**.

        2.  In the **Description** field, enter **Payment Credit card**.

        3.  In the **Bal. Account Type** field, select the **G/L Account**
            option.

        4.  Click the **Bal. Account No.** field, and then click **Select from
            full list**.

        5.  On the **G/L Account List** page, select account number
            **20500/Credit Cards** and click **Edit**. Create a new account if
            you do not find it from the list.

        6.  On the **G/L Account Card** of **20500**, enable **Direct Posting**
            toggle.

        7.  Close the **G/L Account Card**.

        8.  The account number **20500** is automatically filled in the **Bal.
            Account No.** field.

        9.  Click **OK**.

    23. The new code is now automatically filled in the **Payment Method
        Code** field on the customer card.

    24. In the customer card, select **Customer** and then select
        **Dimensions**.

    25. In the opened **Default Dimensions** page, select **+ New**.

    26. Fill in the following fields:

        1.  In the **Dimension Code** field, enter **CUSTOMERGROUP**

        2.  In the **Dimension Value Code** field, enter **SMALL**

        3.  In the **Value Posting** field, select the **Same Code** option.

    27. Close the **Default Dimensions** page.

Task 3: Import customers using data templates
---------------------------------------------

### Scenario

The rest of the domestic customers will be imported using a configuration
package and a configuration template. Make sure the appropriate posting groups
are filled in and that the following requirements are met:

-   All sales documents will be mailed as a pdf-file to the customer’s default
    Email-address and the document will also be stored as a pdf-file.

-   Domestic customers need to pay sales invoices within 30 days of the invoice.

-   The CUSTOMERGROUP dimension needs to be set up as a fixed default on the
    customer card.

The following list of domestic customers is returned to you by Contoso’s super
user.

You will perform

1.  Create and export a configuration package.

2.  Create and assign data template to the configuration package.

3.  Prepare data in excel.

4.  Import and apply the configuration package.

### Steps

1.  Create and export a configuration package.

    1.  Select the Search for page icon in the top-right corner of the page,
        enter `Configuration Packages`, and then choose the related link.

    2.  In the **Configuration Packages** page, click **+ New** to create a new
        configuration package.

    3.  In the **Code** field, enter **CUST**.

    4.  In the **Package Name** field, enter **Customer List**.

    5.  On the **Tables** section of the Config. Package Card, enter a new line
        as follows.

    6.  Open the assist edit button to the right of the **Table ID** field.

    7.  In the window that opens, select the **Customer** table, and click
        **OK**.

    8.  Then press **ENTER** or **TAB**.

    9.  Select the **Dimensions as Columns** check box.

    10. Click **Yes** to add the related dimension tables.

    11. Make sure the customer table line is selected, select **Table** and then
        **Fields**.

    12. Click on **No.**

    13. Click on **Fields** again. On the field list page, first select **Clear
        Included**, to deselect the **Include Field** checkbox for all the
        fields.

    14. Then select the **Include Field** checkbox for the following fields:

        1.  Name

        2.  Address

        3.  City

        4.  Country/Region Code

        5.  Post Code

    15. The **Validate Field** checkbox is automatically selected.

    16. Click **Close**.

    17. In the **Config. Package Card** page, select **Export to Excel**.

    18. Click **Yes** to export the configuration package.

2.  Create and assign data template to the configuration package.

    1.  In the **Tables** section of the Config. Package Card, make sure the
        **Customer** table line is selected.

    2.  Open the assist edit button to the right of the **Data Template** field.

    3.  In the opened **Configuration Templates** page, select **+ New**.

    4.  In the **Config. Template Header** page, fill in the following fields:

        1.  In the **Code** field, enter **CUST DOM**

        2.  In the **Description** field, enter **Domestic customers**

        3.  Open the assist edit button to the right of the **Table ID** field.

        4.  Select the table for **Customers** (ID = 18) and click **OK**.

        5.  Select the **Enabled** check box.

        6.  In the **Lines** section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Gen. Bus. Posting
                Group**.(ID=88)

            3.  In the **Default Value** field, enter **DOMESTIC**

        7.  In the Lines section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Customer Posting
                Group**.(ID=21)

            3.  In the **Default Value** field, enter **DOMESTIC**

        8.  In the Lines section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Document Sending
                Profile**.(ID=11)

            3.  In the **Default Value** field, enter **MAIL&PDF**

        9.  In the Lines section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Payment Terms
                Code**.(ID=27)

            3.  In the **Default Value** field, enter **30 DAYS**

        10. Close the configuration template.

    5.  In the **Configuration Templates** page, make sure the new template for
        domestic customers is selected, and click **OK**.

    6.  The new code is now automatically filled in in the **Data Template**
        field on the configuration package card.

3.  Prepare data in excel.

    1.  Open the exported excel file from the download folder.

    2.  Enter the information as provided by Contoso.

    3.  Save the excel file.

4.  Import and apply the configuration package.

    1.  In the **Configuration Packages** page, select the new configuration
        package for customers and select **Manage** and then **Edit**.

    2.  In the **Config. Package Card** page, select **Import from Excel**.

    3.  Select Click here to browse and select the excel file.

    4.  Click **Open**.

    5.  In the preview page, select **Import**.

    6.  In the **Config. Package Card** page, select **Apply Package**.

    7.  Click **Yes**.

    8.  Click **OK**.
