---
lab:
    title: 'Lab: Set up Accounts Receivable'
    module: 'Module 3: Configure Financials'
---

Hands-on-Lab 3.9: Set Up Accounts Receivable
============================================

Exercise 1: Configure the Sales & Receivables Setup
---------------------------------------------------

### Scenario

Concerning the processing of sales transactions, Contoso’s account manager has
expressed the following requirements:

-   Web shop customers will be numbered separately from other customers. Regular
    customers are numbered C00010 and incremented by 10. Web shop customers are
    numbered CWEB00010 and also incremented by 10.

    *(Remark: The number series for regular customers is already created (CUST)
    and assigned in the Sales & Receivables Setup)*

-   Posted sales invoices are numbered based on the year and month in which they
    are posted. The first sales invoice, as of January 1st 2022, will be posted
    with the number S22/01/0001. The next month will be S22/02/0001 and so on.

-   A separate g/l account 40300 is setup to record invoice discounts only that
    were given to the customer. Line discounts are also given, but considered as
    part of the net sales price and thus not posted separately from the normal
    sales account.

-   Contoso works with a credit insurer, who provides credit limits for each
    customer. When this limit is reached, sales people have to communicate with
    the finance department before going ahead with the sale.

### Tasks

1.  Set up and assign number series

2.  Complete discount posting setup

3.  Activate credit limit warning

### Steps

1.  Set up and assign number series.

    1.  In the **Sales & Receivables Setup** page, go to the **Number Series**
        FastTab.

    2.  In the **Customer Nos.** field, the value CUST is already filled in.
        Click on the Look Up Value button and select New.

    3.  In the opened **No. Series List** page, fill in the following fields:

        1.  In the **Code** field, enter CUST WEB

        2.  In the **Description** field, enter ‘Customers Web Shop’.

        3.  Select the **Default Nos.** check box.

    4.  Select **Navigate** and then select **Lines**.

    5.  In the opened **No. Series Lines** page, select **New**.

        1.  Leave the **Starting Date** field blank.

        2.  In the **Starting No.** field, enter CWEB0001.

        3.  In the **Increment-by No.** field, enter the value ‘10’.

    6.  Close the **No. Series Lines** page.

    7.  In the opened **No. Series List** page, select the number series CUST.

    8.  Select **Navigate** and then select **Relationships**.

    9.  In the **No. Series Relationships** page, select **New**.

    10. In the **Series Code** field, enter CUST WEB.

    11. Close the **No. Series Relationships** page.

    12. Close the **No. Series List** page, by clicking **OK**.

    13. You are now back in the **Sales & Receivables Setup** page, on the
        **Number Series** FastTab.

    14. In the **Posted Invoice Nos.** field, the value S-INV+ is already filled
        in. Click on the Look Up Value button and then click **Select from full
        list.**

    15. In the opened **No. Series List** page, the number series S-INV+ is
        automatically selected.

    16. Select **Navigate** and then select **Lines**.

    17. In the opened **No. Series Lines** page, select **New**.

        1.  In the **Starting Date** field, enter 1/1/2022.

        2.  In the **Starting No.** field, enter S22/01/0001.

        3.  In the **Increment-by No.** field, leave the value ‘1’.

    18. In the opened **No. Series Lines** page, select **New**.

        1.  In the **Starting Date** field, enter 2/1/2022.

        2.  In the **Starting No.** field, enter S22/02/0001.

        3.  In the **Increment-by No.** field, leave the value ‘1’.

    19. Close the **No. Series Lines** page.

    20. Close the **No. Series List** page, by clicking **OK**.

    21. The number series S-INV+ remains filled in in the **Posted Invoice
        Nos.** field, in the **Sales & Receivables Setup** page.

2.  Complete discount posting setup.

    1.  In the **Sales & Receivables Setup** page, go to the **General**
        FastTab.

    2.  In the **Discount Posting** field, select the **Invoice Discounts**
        option.

    3.  In the **General Posting Setup** page, for each possible combination of
        **Gen. Bus. Posting Group** and **Gen. Prod. Posting Group**, make sure
        the **Sales Inv. Disc. Account** field is filled in with the value
        40300.

3.  Activate credit limit warning

    1.  In the **Sales & Receivables Setup** page, go to the **General**
        FastTab.

    2.  In the **Credit Warnings** field, select the **Credit Limit** option.

Exercise 2: Create and configure customers
------------------------------------------

### Scenario

Based on the chart of accounts, you will set up the different customer posting
groups. With their fast growing business abroad, they want to keep track of
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

You need to create this customer manually. (You can use the CUSTOMER COMPANY
customer template, and then alter the customer setup as necessary.)

### Tasks

1.  Set up a Customer Posting Group.

2.  Create and configure a new customer.

### Steps

1.  Set up a Customer Posting Group

    1.  In the **Customer Posting Groups** page, select **New**.

    2.  In the **Customer Posting Group Card** page, fill in the following
        fields:

        1.  In the **Code** field, fill in FOREIGN.

        2.  In the **Description** field, fill in ‘Foreign customers’.

        3.  In the **Receivables Account** field, fill in 10450.

        4.  Close the page.

    3.  In the **Customer Posting Groups** page, select **New**.

    4.  In the **Customer Posting Group Card** page, fill in the following
        fields:

        1.  In the **Code** field, fill in INTERCOMPANY.

        2.  In the **Description** field, fill in ‘Intercompany customers’.

        3.  In the **Receivables Account** field, fill in 10475.

        4.  Close the page.

    5.  From the **Customer Posting Groups** page, copy the other g/l accounts
        from the DOMESTIC customer posting group to the FOREIGN and INTERCOMPANY
        customer posting groups using F8. Copy the following fields:

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

    1.  In the **Customers** page, select **New**.

    2.  On the **Select a template for a new customer** page, choose the
        CUSTOMER COMPANY template and click **OK**.

    3.  Go to the **General** FastTab and click **Show more**.

    4.  Open the assist edit button to the right of the **No.** field.

    5.  In the window that opens, select the number series for web shop
        customers CUST WEB and click **OK**.

    6.  Click **Yes** to change the customer no. and update any related records.

    7.  In the **Name** field, enter ‘Generic EU web shop’.

    8.  In the **Document Sending Profile** field, click on the Look Up Value
        button and click **New**.

    9.  In the opened **Document Sending Profile** card page, fill in the
        following fields:

        1.  In the **Code** field, enter MAIL&PDF.

        2.  In the **Description** field, enter ‘Mail & PDF’.

        3.  In the **Email** field, select the **Yes (Use Default Settings)**
            option.

        4.  The **Email Attachment** field is automatically set to the **PDF**
            option.

        5.  In the **Disk** field, select the **PDF** option.

        6.  Click **OK**.

    10. The new code is now automatically filled in in the **Document Sending
        Profile** field on the customer card.

    11. Go to the **Invoicing** FastTab.

    12. In the **Gen. Bus. Posting Group** field, change the DOMESTIC value to
        EU.

    13. The **VAT Bus. Posting Group** field is automatically filled in with the
        value EU.

        *(Remark: The value of this field can be seen through Page Inspection –
        Ctrl + Alt + F1)*

    14. In the **Customer Posting Group**, change the DOMESTIC value to FOREIGN.

    15. Go to the **Payments** FastTab and click on **Show more**.

    16. In the **Payment Terms Code** field, click on the Look Up Value button
        and click **New**.

    17. In the opened **Payment Terms** page, fill in the following fields:

        1.  In the **Code** field, enter 0 DAYS.

        2.  In the **Due Date Calculation** field, enter 0D.

        3.  In the **Description** field, enter ‘Pay before delivery’.

        4.  Click **OK**.

    18. The new code is now automatically filled in in the **Payment Terms
        Code** field on the customer card.

    19. In the **Payment Method Code** field, click on the Look Up Value button
        and click **New**.

    20. In the opened **Payment Methods** page, fill in the following fields:

        1.  In the **Code** field, enter CREDITCARD.

        2.  In the **Description** field, enter Payment Creditcard.

        3.  In the **Bal. Account Type** field, select the **G/L Account**
            option.

        4.  In the **Bal. Account No.** field, enter 20500. (*Make sure the
            Direct Posting check box is selected on the g/l account card)*

        5.  Click **OK**.

    21. The new code is now automatically filled in in the **Payment Method
        Code** field on the customer card.

    22. In the customer card, select **Customer** and then select
        **Dimensions**.

    23. In the opened **Default Dimensions** page, select **New**.

    24. Fill in the following fields:

        1.  In the **Dimension Code** field, enter CUSTOMERGROUP

        2.  In the **Dimension Value Code** field, enter SMALL

        3.  In the **Value Posting** field, select the **Same Code** option.

    25. Close the **Default Dimensions** page.

Exercise 3: Import customers using data templates
-------------------------------------------------

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

![](media/lab3_6_domestic_customers.png)

### Tasks

1.  Create and export a configuration package.

2.  Create and assign data template to the configuration package.

3.  Prepare data in excel.

4.  Import and apply the configuration package.

### Steps

1.  Create and export a configuration package.

    1.  In the **Configuration Packages** page, click **New** to create a new
        configuration package.

    2.  In the **Code** field, enter CUST.

    3.  In the **Package Name** field, enter Customer List.

    4.  On the **Tables** section of the Config. Package Card, enter a new line
        as follows.

    5.  Open the assist edit button to the right of the **Table ID** field.

    6.  In the window that opens, select the **Customer** table and click
        **OK**.

    7.  Then press ENTER or TAB.

    8.  You will be asked to check related tables, click **No**.

    9.  Select the **Dimensions as Columns** check box.

    10. Click **Yes** to add the related dimension tables.

    11. Make sure the customer table line is selected, select **Table** and then
        **Fields**.

    12. On the field list page, first select **Clear Included**, to deselect the
        **Include Field** checkbox for all the fields.

    13. Then select the **Include Field** checkbox for the following fields:

        1.  Name

        2.  Address

        3.  City

        4.  Country/Region Code

        5.  Post Code

    14. The **Validate Field** checkbox is automatically selected.

    15. Click **Close**.

    16. In the **Config. Package Card** page, select **Export to Excel**.

    17. Click **Yes** to export the configuration package.

2.  Create and assign data template to the configuration package.

    1.  In the **Tables** section of the Config. Package Card, make sure the
        customer table line is selected.

    2.  Open the assist edit button to the right of the **Data Template** field.

    3.  In the opened **Configuration Templates** page, select **New**.

    4.  In the **Config. Template Header** page, fill in the following fields:

        1.  In the **Code** field, enter CUST DOM

        2.  In the **Description** field, enter ‘Domestic customers’

        3.  Open the assist edit button to the right of the **Table ID** field,
            select the table for customers (ID = 18) and click **OK**.

        4.  Select the **Enabled** check box.

        5.  In the **Lines** section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Gen. Bus. Posting Group**.

            3.  In the **Default Value** field, enter DOMESTIC

        6.  In the **Lines** section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Customer Posting Group**.

            3.  In the **Default Value** field, enter DOMESTIC

        7.  In the **Lines** section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Document Sending Profile**.

            3.  In the **Default Value** field, enter MAIL&PDF

        8.  In the **Lines** section on the page, create the following line:

            1.  In the **Type** field, enter **Field**.

            2.  In the **Field Name** field, enter **Payment Terms Code**.

            3.  In the **Default Value** field, enter 30 DAYS

        9.  Close the configuration template.

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

    3.  Click **Choose…** and select the excel file.

    4.  Click **Open**.

    5.  In the preview page, select **Import**.

    6.  Make sure the customer table line is selected, select **Functions** and
        then **Apply data**.

    7.  Click **Yes**.

    8.  Click **OK**.
