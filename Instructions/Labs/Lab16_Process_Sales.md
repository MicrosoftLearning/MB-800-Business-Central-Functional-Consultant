Exercise 16: Process Sales
==========================

Task 1: Process a sales from quote to invoice
---------------------------------------------

### Scenario

Through the European web shop a new company has requested a quote for several
monitors.

Since it is a company, and not a private person, first a Contoso account is
created, which is entered in Business Central as a contact card. The company
Francematic is located in France, at the following address: 19 Boulevard
Commanderie, FR-78370 PLAISIR.

You need to prepare a customer template to be able to convert EU contacts into
EU customers, using the correct posting group information, sales prices and line
discount and needs to pay before delivery.

On February 16th, 2023, a quote is created by Benjamin Chiu for the following
items:

-   1 box of the 15” flat panels, at the current price of \$ 4,800.00 a box with
    a 6% discount for all medium-sized companies.

-   3 pieces of the 17” monitor, at the current price of \$ 700.00 a piece with
    a 6% discount for all medium-sized companies.

The potential customer now has 10 days to either accept or turn down the
proposal.

On February 22nd, 2023, Francematic accepts the sales quote and the quote is
turned into an order.

The items are shipped to the customer on 2 different dates:

-   On February 27th, 2023, the 15” flat panels are delivered.

-   On February 28th, 2023, the 17” monitors are delivered.

On March 1st, 2023, the sales invoice is created and send to the customer.

You will perform

1.  Create a contact.

2.  Create a sales quote for a contact.

3.  Process the quote into an order.

4.  Partially ship items from the order.

5.  Create a posted sales invoice from the sales order.

### Steps

1.  Create a contact.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Contacts**, and then choose the related link.

    2.  In the **Contacts** list page, select **+ New**.

    3.  On the **General** FastTab, fill in the following fields:

        1.  In the **Name** field, enter **Francematic**.

        2.  In the **Type** field, leave the default value **Company**.

    4.  On the **Communication** FastTab, fill in the following fields:

        1.  In the **Address** field, enter **19 Boulevard Commanderie**.

        2.  In the **Country/Region Code** field, enter **FR**.

        3.  In the **ZIP Code** field, enter **FR-78370**.

        4.  The **City** field is automatically filled in with the value
            **PLAISIR**.

    5.  On the **Foreign Trade** FastTab, leave the **Currency Code** field
        blank.

2.  Create a sales quote for a contact.

    1.  On the **Contacts** list page, select the new contact **Francematic**.

    2.  Select **Home** and then select **Create Sales Quote**.

    3.  Click **Yes** for selecting a customer template.

    4.  Select the **CUSTOMER COMPANY** template and click **OK**.

    5.  A new sales quote is created.

    6.  In the **General** FastTab, click **Show more** and then fill in the
        following fields:

        1.  In the **Order Date** and **Document Date** field, enter
            **2/15/2023**.

        2.  In the **Quote Valid To Date** field, enter **2/25/2023**.

        3.  In the **Salesperson Code** field, enter **BC**.

    7.  On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1002** for the **15” flat panels**.

        3.  In the **Location Code** field, enter **EUROP**.

        4.  In the **Unit of Measure Code** field, enter **BOX**.

        5.  In the **Quantity** field, enter **1**.

        6.  In the **Unit Price Excl. Tax** field, enter **4,800.00**.

        7.  In the **Line Discount %** field, enter **6**.

        8.  In the **Tax Group Code**, enter **NONTAXABLE**.

    8.  On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1003 for the 17” flat panels**.

        3.  In the **Location Code** field, enter **EUROP**.

        4.  In the **Unit of Measure Code** field, leave the default value
            **PCS**.

        5.  In the **Quantity** field, enter **3**.

        6.  In the **Unit Price Excl. Tax** field, enter **700.00**.

        7.  In the **Line Discount %** field, enter **6**.

        8.  In the **Tax Group Code**, enter **NONTAXABLE**.

3.  Process the quote into an order.

    1.  On the **Sales Quote** card page, change the **Order Date** field to
        **2/22/2023**.

    2.  Select **Home** and then select **Make Order**.

    3.  Click **Yes**.

    4.  Click **Yes** to create a customer card for contact **Francematic**.

    5.  Click **OK**.

    6.  Click **Yes** to open the sales order.

4.  Partially ship items from the order.

    1.  On the **Sales Order** card page, on the **General** FastTab, in the
        **Posting Date** field, enter **2/27/2023**.

    2.  On the **Lines** FastTab, select the line for the **17” monitors**.

    3.  In the **Qty. to Ship** field, remove the value, and leave the field
        blank.

    4.  Select **Home** and then select **Post**.

    5.  Select the **Ship** option and click **OK**.

    6.  Select **OK**.

    7.  On the **General** FastTab, in the **Posting Date** field, enter
        **2/28/2023**.

    8.  Select **Home** and then select **Post**.

    9.  Select the **Ship** option and click **OK**.

    10. Select **OK**.

5.  Create a posted sales invoice from the sales order.

    1.  On the **Sales Order** card page, on the **General** FastTab, in the
        **Posting Date** field, enter **3/1/2023**.

    2.  Select **Home** and then select **Post**.

    3.  Select the **Invoice** option and click **OK**.

    4.  Select **No**.

6.  Review the posted sales invoice.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Posted Sales Invoices**, and then choose the related link.

    2.  In the **Posted Sales Invoices** list page, select the invoice for
        customer **Francematic**.

    3.  Select **Actions** and then select **Find entries**.

    4.  Select the line for G/L entries and select **Show Related Entries**.

    5.  Close the **G/L entries** page.

    6.  Close the **Find Entries** page.

Task 2: Process a sales invoice for multiple orders
---------------------------------------------------

### Scenario

During the month January the web shop sales has been picking up and a lot of
items were shipped to private customers.

First record a couple of these sales orders and shipments for the Generic EU web
shop customer as follows:

| Order & Delivery Date | Reference       | Shipment Address | Qty.  | Item    |
|-----------------------|-----------------|------------------|-------|---------|
| 1/5/2023              | Private sale DK | PICK-UP-DK       | 2 PCS | CHW1002 |
| 1/6/2023              | Private sale BE | PICK-UP-BE       | 1 BOX | CHW1002 |
| 1/9/2023              | Private sale FR | PICK-UP-FR       | 5 PCS | CHW1003 |

At the end of March 2023, 1 combined invoice is created for all private sales.
You must now create this sales invoice for the Generic EU web shop customers,
containing all shipments of January, including the 5% web shop discount for the
month January.

You will perform

1.  Create several sales orders and shipments.

2.  Use the Combine Shipments function to create sales invoices.

### Steps

1.  Create several sales orders and shipments.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Customers**, and then choose the related link.

    2.  On the **Customers** list page, select the **Generic EU web shop**
        customer.

    3.  Select **New Document** and then select **Sales Order**.

    4.  On the opened **Sales Order** card page, on the **General** FastTab,
        click **Show more** and then fill in the following fields:

        1.  In the **Order Date** field, enter **1/5/2023**.

        2.  In the **Posting Date** field, enter **3/6/2023**.

        3.  In the **Your Reference** field, enter **Private sale DK**.

    5.  On the **Shipping and Billing** FastTab, fill in the following fields:

        1.  In the **Ship-to** field, select the **Alternate Shipping Address**
            option.

        2.  On the opened **Ship-to Address** List page, select PICK-UP-DK and
            click **OK**.

        3.  Select the **Combine Shipments** checkbox.

    6.  On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1002**.

        3.  In the **Location Code** field, the value **EUROP** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value **PCS** is
            automatically filled in.

        5.  In the **Quantity** field, enter **2**.

        6.  In the **Tax Group Code** field, enter **NONTAXABLE**.

    7.  Select **Home** and then select **Post**.

    8.  Select the **Ship** option and click **OK**.

    9.  Click **OK** for the sales order to be placed in a job queue.

    10. Close the **Sales Order** page.

    11. On the **Customers** list page, select the **Generic EU web shop**
        customer.

    12. Select **New Document** and then select **Sales Order**.

    13. On the opened **Sales Order** card page, on the **General** FastTab,
        click **Show more** and then fill in the following fields:

        1.  In the **Order Date** field, enter **1/6/2023**.

        2.  In the **Posting Date** field, enter **3/7/2023**.

        3.  In the **Your Reference** field, enter **Private sale BE**.

    14. On the **Shipping and Billing** FastTab, fill in the following fields:

        1.  In the **Ship-to** field, select the **Alternate Shipping Address**
            option.

        2.  On the opened **Ship-to Address** List page, select PICK-UP-BE and
            click **OK**.

        3.  Select the **Combine Shipments** checkbox.

    15. On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1002**.

        3.  In the **Location Code** field, the value **EUROP** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, enter **BOX**.

        5.  In the **Quantity** field, enter **1**.

        6.  In the **Tax Group Code**, enter **NONTAXABLE**.

    16. Select **Home** and then select **Post**.

    17. Select the **Ship** option and click **OK**.

    18. Click **OK** for the sales order to be placed in a job queue.

    19. Close the **Sales Order** page.

    20. On the **Customers** list page, select the **Generic EU web shop**
        customer.

    21. Select **New Document** and then select **Sales Order**.

    22. On the opened **Sales Order** card page, on the **General** FastTab,
        click **Show more** and then fill in the following fields:

        1.  In the **Order Date** field, enter **1/9/2023**.

        2.  In the **Posting Date** field, enter **3/8/2023**.

        3.  In the **Your Reference** field, enter **Private sale FR**.

    23. On the **Shipping and Billing** FastTab, fill in the following fields:

        1.  In the **Ship-to** field, select the **Alternate Shipping Address**
            option.

        2.  On the opened **Ship-to Address** List page, select **PICK-UP-FR**
            and click **OK**.

        3.  Select the **Combine Shipments** checkbox.

    24. On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1003**.

        3.  In the **Location Code** field, the value **EUROP** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field , the value **PCS** is
            automatically filled in.

        5.  In the **Quantity** field, enter **5**.

        6.  In the **Tax Group Code** field, enter **NONTAXABLE**.

    25. Select **Home** and then select **Post**.

    26. Select the **Ship** option and click **OK**.

    27. Click **OK** for the sales order to be placed in a job queue.

    28. Close the **Sales Order** page.

2.  Use the Combine Shipments function to create sales invoices.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Combine Shipments**, and then choose the related link.

    2.  Open the **Combine Shipments** task.

    3.  In the **Posting Date** and **Document Date** field, enter **3/8/2023**.

    4.  Select the **Calc. Inv. Discount** checkbox.

    5.  Select the **Post Invoices** checkbox.

    6.  In the **Sell-to Customer No.** filter, enter **CWEB0001**.

    7.  Click **OK**.

    8.  Click **OK**.

Task 3: Correct a posted sales invoice
--------------------------------------

### Scenario

The new customer Francematic complaint that only 2 of the 3 17” monitors were
delivered.

You need to make a sales credit memo on March 6th, 2023, to refund 1 piece of
this item.

You will perform

1.  Correct a posted sales invoice

### Steps

1.  Correct a posted sales invoice

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Posted Sales Invoices**, and then choose the related link.

    2.  On the **Posted Sales Invoices** list page, select the invoice for
        customer Francematic.

    3.  Select **Correct** and then select **Create Corrective Credit Memo**.

    4.  On the opened sales credit memo, on the **General** FastTab, click
        **Show more** and then enter **3/6/2023** in the **Posting Date** field.

    5.  On the **Lines** section, delete the line for the 15” flat panels.

    6.  On the **Lines** section, select the line for the 17” monitors.

    7.  Change the **Quantity** field from **3** to **1**.

    8.  Select **Home** and then select **Post**.

    9.  Click **Yes**.

    10. Click **No**.
