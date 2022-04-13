
---
lab:
    title: 'Lab: Process Sales'
    module: 'Module 5: Operations'
---

Hands-on-Lab 5.2: Process Sales
===============================

Exercise 1: Complete the customer card
--------------------------------------

### Scenario

As the functional consultant, you are collecting more information about the
sales process, and more particularly about the customers who are buying your
products and the conditions surrounding delivery.

In order to deliver the computer hardware items from the European warehouse to
the European customers, Contoso uses DHL as a shipping agent. Web shop customers
who are end-users will have the option to choose between home delivery or
delivery at a pick-up point.

The following different pick-up points are set up as shipping addresses on the
webshop customer (CWEB0001):

-   PICK-UP DK: Carl Blochs Gade 7, DK-8000 Arhus C – contact: Hr. Jonathan
    Mollerup

-   PICK-UP BE: Binkkampen 33, BE-1020 BRUSSEL – contact: Dhr. Luc van Vugt

-   PICK-UP FR: 34 Avenue Parmentier, FR-75000 PARIS – contact: M. Jean E.
    TRENARY

Since this is a generic customer, different orders are never combined into one
shipment. It is however possible that one order needs to be shipped parts
because of item availability. This should be under rare circumstances, since
Contoso has stated to his customers to guarantee a maximum delivery time within
2 days, which is compliant with DHL’s standard shipping service and time.

In the domestic areas sales activities are performed by sales representatives
who each have their set of customers. All transactions need to be assigned to a
specific sales person as follows:

-   C00010 Spotsmeyer’s Furnishings is a customer from Annette Hill

-   C00020 Progressive Home Furnishings is a customer from John Roberts

-   C00030 New Concepts Furniture is a customer from Peter Saddow

You will have to create all sales people. Also don’t forget to assign the
SALESPEOPLE dimension to each sales person.

-   Annette Hill

-   Bart Duncan

-   Debra L. Core

-   John Roberts

-   Mary A. Dempsey

-   Peter Saddow

-   Richard Lum

### Tasks

1.  Create a shipping address for the customer.

2.  Specify shipping information.

3.  Set up and assign a salesperson

### Steps

1.  Create a shipping address for the customer.

    1.  On the **Customers** list page, select the web shop customer (CWEB0001).

    2.  To open the customer card, select **Manage** and then select **Edit**.

    3.  In the customer card, select **Related**, then select **Customer** and
        then **Ship-to Addresses**.

    4.  In the opened **Ship-to Address** List page, select **New**.

    5.  In the opened ship-to addresses card, fill in the following fields:

        1.  In the **Code** field, enter PICK-UP DK

        2.  In the **Name** field, the value ‘Generic EU web shop’ is
            automatically filled in. Replace with ‘Pick-up point Denmark’.

        3.  In the **Address** field, enter ‘Carl Blochs Gade 7’.

        4.  In the **City** field, enter ‘Arhus C’

        5.  In the **ZIP Code** field, the value ‘DK-8000’ is automatically
            filled in.

        6.  In the **Country/Region Code** field, the value ‘DK’ is
            automatically filled in.

        7.  In the **Contact** field, enter ‘Hr. Jonathan Mollerup’.

    6.  Close the ship-to address card.

    7.  In the **Ship-to Address List** page, select **New**.

    8.  In the opened ship-to addresses card, fill in the following fields:

        1.  In the **Code** field, enter PICK-UP BE

        2.  In the **Name** field, the value ‘Generic EU web shop’ is
            automatically filled in. Replace with ‘Pick-up point Belgium’.

        3.  In the **Address** field, enter ‘Binkkampen 33’.

        4.  In the **City** field, enter ‘Brussel’

        5.  In the **ZIP Code** field, enter ‘BE-1020’.

        6.  In the **Country/Region Code** field, the value ‘BE’ is
            automatically filled in.

        7.  In the **Contact** field, enter ‘Dhr. Luc van Vugt’.

    9.  Close the ship-to address card.

    10. In the opened **Ship-to Address** List page, select **New**.

    11. In the opened ship-to addresses card, fill in the following fields:

        1.  In the **Code** field, enter PICK-UP FR

        2.  In the **Name** field, the value ‘Generic EU web shop’ is
            automatically filled in. Replace with ‘Pick-up point France’.

        3.  In the **Address** field, enter ‘34 Avenue Parmentier’.

        4.  In the **City** field, enter ‘Paris’

        5.  In the **ZIP Code** field, the value ‘FR-75000’ is automatically
            filled in.

        6.  In the **Country/Region Code** field, the value ‘FR’ is
            automatically filled in.

        7.  In the **Contact** field, enter ‘M. Jean E. TRENARY’.

    12. Close the ship-to address card.

    13. Close the **Ship-to Address List** page.

2.  Specify shipping information.

    1.  On the customer card for the generic web shop customer (CWEB0001), go to
        the **Shipping** FastTab.

    2.  Leave the **Ship-to Code** field blank.

    3.  In the **Location Code** field, enter EUROP.

    4.  In the **Agent** field, enter DHL

    5.  In the **Agent Service** field, enter STANDARD

    6.  In the **Shipping Time** field, the value 2D is automatically filled in.

3.  Set up and assign a salesperson

    1.  On the **Salespeople/Purchasers** list page, select **New**.

    2.  On the opened salesperson card, fill in the following fields:

        1.  In the **Code** field, enter AH

        2.  In the **Name** field, enter Annette Hill.

        3.  In the **Salespeople Code** field, enter AH to assign

    3.  On the opened salesperson card, select **Salesperson**, and then select
        **Dimensions**.

    4.  On the opened **Default Dimensions** page, select **New**.

    5.  On the new line, fill in the following fields:

        1.  In the **Dimension Code** field, enter SALESPEOPLE

        2.  In the **Dimension Value Code** field, enter AH

        3.  In the **Value Posting** field, select the **Same Code** option.

        4.  Close the page.

    6.  Close the salesperson card.

    7.  Repeat steps a. to f. for the other salespeople.

        *(Remark: for further exercise purposes it is sufficient if you create
        John Roberts, Peter Saddow and Debra L. Core.)*

    8.  On the **Customers** list page, select customer Spotsmeyer’s Furnishings
        (C00010)

    9.  To open the customer card, select **Manage** and then select **Edit**.

    10. On the **General** FastTab, in the **Salesperson Code** field, enter AH

    11. Go to the next customer card for customer Progressive Home Furnishings.

    12. On the **General** FastTab, in the **Salesperson Code** field, enter JR

    13. Go to the next customer card for customer New Concepts Furniture.

    14. On the **General** FastTab, in the **Salesperson Code** field, enter PS

Exercise 2: Process a sales from quote to invoice
-------------------------------------------------

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

On January 16th, 2022, a quote is created by Debra L. Core for the following
items:

-   1 box of the 15” flat panels, at the current price of LCY 4,800.00 a box
    with a 6% discount for all medium-sized companies.

-   3 pieces of the 17” monitor, at the current price of LCY 700.00 a piece with
    a 6% discount for all medium-sized companies.

The potential customer now has 10 days to either accept or turn down the
proposal.

On January 22nd, 2022 Francematic accepts the sales quote and the quote is
turned into an order.

The items are shipped to the customer on 2 different dates:

-   On January 25th, 2022, the 15” flat panels are delivered.

-   On January 27th, 2022, the 17” monitors are delivered.

On January 28th, 2022, the sales invoice is created and send to the customer.

### Tasks

1.  Create a contact.

2.  Create a customer template.

3.  Create a sales quote for a contact.

4.  Process the quote into an order.

5.  Partially ship items from the order.

6.  Create a posted sales invoice from the sales order.

### Steps

1.  Create a contact.

    1.  In the **Contacts** list page, select **New**.

    2.  On the **General** FastTab, fill in the following fields:

        1.  In the **Name** field, enter ‘Francematic’.

        2.  In the **Type** field, leave the default value **Company**.

    3.  On the **Communication** FastTab, fill in the following fields:

        1.  In the **Address** field, enter ‘19 Boulevard Commanderie’.

        2.  In the **Country/Region Code** field, enter FR.

        3.  In the **ZIP Code** field, enter FR-78370.

        4.  The **City** field is automatically filled in with the value
            PLAISIR.

    4.  On the **Foreign Trade** FastTab, leave the **Currency Code** field
        blank.

2.  Create a customer template

    1.  On the **Customer Templates** page, select **New**.

    2.  In the opened customer template card, fill in the following fields:

        1.  In the **Code** field, enter CUST EU.

        2.  In the **Description** field, enter ‘Customer EU’.

        3.  In the **Contact Type** field, leave the default value ‘Company’.

        4.  Leave the **Currency Code** field blank.

        5.  In the **Gen. Bus. Posting Group** field, enter EU.

        6.  In the **Customer Posting Group** field, enter FOREIGN.

        7.  In the **Customer Price Group** field, enter EU.

        8.  In the **Customer Disc. Group** field, enter MEDIUM.

        9.  In the **Payment Terms Code** field, enter ‘0 DAYS’.

        10. Select **Dimensions**, and fill in the following fields:

            1.  In the **Dimension Code** field, enter CUSTOMERGROUP

            2.  In the **Dimension Value Code** field, enter MEDIUM

        11. Close the **Default Dimensions** page and then close the customer
            template card.

3.  Create a sales quote for a contact.

    1.  On the **Contacts** list page, select the new contact Francematic.

    2.  Select **Process** and then select **Create Sales Quote**.

    3.  A new sales quote is created.

    4.  In the **General** FastTab, fill in the following fields:

        1.  In the **Order Date** and **Document Date** field, enter 1/15/2022.

        2.  In the **Quote Valid To Date** field, enter 1/25/2022.

        3.  In the **Salesperson Code** field, enter DC.

    5.  On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter CHW1002 for the 15” flat panels.

        3.  In the **Location Code** field, enter EUROP.

        4.  In the **Unit of Measure Code** field, enter BOX.

        5.  In the **Quantity** field, enter 1.

        6.  In the **Unit Price Excl. Tax** field, the value 4,800.00 is
            automatically filled in.

        7.  In the **Line Discount %** field, the value ‘6’ is automatically
            filled in.

    6.  On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter CHW1003 for the 17” flat panels.

        3.  In the **Location Code** field, enter EUROP.

        4.  In the **Unit of Measure Code** field, leave the default value PCS.

        5.  In the **Quantity** field, enter 3.

        6.  In the **Unit Price Excl. Tax** field, the value 700.00 is
            automatically filled in.

        7.  In the **Line Discount %** field, the value ‘6’ is automatically
            filled in.

4.  Process the quote into an order.

    1.  On the **Sales Quote** card page, change the **Order Date** field to
        1/22/2022.

    2.  Select **Process** and then select **Make Order**.

    3.  Click **Yes**.

    4.  Click **Yes** to create a customer card for contact Francematic.

    5.  Click **OK**.

    6.  Click **Yes** to open the sales order.

5.  Partially ship items from the order.

    1.  On the **Sales Order** card page, on the **General** FastTab, in the
        **Posting Date** field, enter 1/25/2022.

    2.  On the **Lines** FastTab, select the line for the 17” monitors.

    3.  In the **Qty. to Ship** field, remove the value, and leave the field
        blank.

    4.  Select **Posting** and then select **Post**.

    5.  Select the **Ship** option and click **OK**.

    6.  On the **General** FastTab, in the **Posting Date** field, enter
        1/27/2022.

    7.  Select **Posting** and then select **Post**.

    8.  Select the **Ship** option and click **OK**.

6.  Create a posted sales invoice from the sales order.

    1.  On the **Sales Order** card page, on the **General** FastTab, in the
        **Posting Date** field, enter 1/28/2022.

    2.  Select **Posting** and then select **Post**.

    3.  Select the **Invoice** option and click **OK**.

    4.  Click **OK** to open the posted sales invoice.

7.  Review the posted sales invoice.

    1.  In the opened posted sales invoice, select **Invoice** and then select
        **Find entries**.

    2.  Select the line for G/L entries sand select **Show Related Entries**.

![](https://github.com/MicrosoftLearning/MB-800-Business-Central-Functional-Consultant/blob/master/Instructions/Labs/media/MB800_2021_Lab%205.2_general_ledger_entries.png)

1.  Close the **G/L entries** page.

2.  Close the **Find Entries** page.

Exercise 3: Process a sales invoice for multiple orders
-------------------------------------------------------

### Scenario

During the month January the web shop sales has been picking up and a lot of
items were shipped to private customers.

First record a couple of these sales orders and shipments for the generic EU
customer as follows:

| Order & Delivery Date | Reference       | Shipment Address | Qty.  | Item    |
|-----------------------|-----------------|------------------|-------|---------|
| 1/26/2022             | Private sale DK | PICK-UP-DK       | 2 PCS | CHW1002 |
| 1/27/2022             | Private sale BE | PICK-UP-BE       | 1 BOX | CHW1002 |
| 1/28/2022             | Private sale FR | PICK-UP-FR       | 5 PCS | CHW1003 |

At the end of the month, 1 combined invoice is created for all private sales.
You must now create this sales invoice for the generic EU customers, containing
all shipments of January, including the 5% web shop discount for the month
January.

*Remark: for exercise purposes we are not taken any VAT into consideration.
Therefor you will have to remove the VAT Business Posting Group on each sales
order.*

### Tasks

1.  Create several sales orders and shipments.

2.  Use the Combine Shipments function to create sales invoices.

### Steps

1.  Create several sales orders and shipments.

    1.  On the **Customers** list page, select the generic EU customer.

    2.  Select **New Document** and then select **Sales Order**.

    3.  On the opened **Sales Order** card page, on the **General** FastTab,
        fill in the following fields:

        1.  In the **Order Date** field, enter 1/26/2022.

        2.  In the **Posting Date** field, enter 1/26/2022.

        3.  In the **Your Reference** field, enter ‘Private sale DK’.

    4.  On the **Shipping and Billing** FastTab, fill in the following fields:

        1.  In the **Ship-to** field, select the **Alternate Shipping Address**
            option.

        2.  On the opened **Ship-to Address** List page, select PICK-UP-DK and
            click **OK**.

        3.  Select the **Combine Shipments** checkbox.

    5.  *On the Invoice Details FastTab, fill in the following fields:*

        1.  *In the VAT Bus. Posting Group field, remove the value EU and leave
            blank.*

    6.  On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter CHW1002.

        3.  In the **Location Code** field, the value EUROP is automatically
            filled in.

        4.  In the **Unit of Measure Code** field , the value PCS is
            automatically filled in.

        5.  In the **Quantity** field, enter ‘2’.

    7.  Select **Posting** and then select **Post**.

    8.  Select the **Ship** option and click **OK**.

    9.  Close the **Sales Order** page.

    10. On the **Customers** list page, select the generic EU customer.

    11. Select **New Document** and then select **Sales Order**.

    12. On the opened **Sales Order** card page, on the **General** FastTab,
        fill in the following fields:

        1.  In the **Order Date** field, enter 1/28/2022.

        2.  In the **Posting Date** field, enter 1/28/2022.

        3.  In the **Your Reference** field, enter ‘Private sale BE’.

    13. On the **Shipping and Billing** FastTab, fill in the following fields:

        1.  In the **Ship-to** field, select the **Alternate Shipping Address**
            option.

        2.  On the opened **Ship-to Address** List page, select PICK-UP-BE and
            click **OK**.

        3.  Select the **Combine Shipments** checkbox.

    14. *On the Invoice Details FastTab, fill in the following fields:*

        1.  *In the VAT Bus. Posting Group field, remove the value EU and leave
            blank.*

    15. On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter CHW1002.

        3.  In the **Location Code** field, the value EUROP is automatically
            filled in.

        4.  In the **Unit of Measure Code** field , enter BOX.

        5.  In the **Quantity** field, enter ‘1’.

    16. Select **Posting** and then select **Post**.

    17. Select the **Ship** option and click **OK**.

    18. Close the **Sales Order** page.

    19. On the **Customers** list page, select the generic EU customer.

    20. Select **New Document** and then select **Sales Order**.

    21. On the opened **Sales Order** card page, on the **General** FastTab,
        fill in the following fields:

        1.  In the **Order Date** field, enter 1/29/2022.

        2.  In the **Posting Date** field, enter 1/29/2022.

        3.  In the **Your Reference** field, enter ‘Private sale FR’.

    22. On the **Shipping and Billing** FastTab, fill in the following fields:

        1.  In the **Ship-to** field, select the **Alternate Shipping Address**
            option.

        2.  On the opened **Ship-to Address** List page, select PICK-UP-FR and
            click **OK**.

        3.  Select the **Combine Shipments** checkbox.

    23. *On the Invoice Details FastTab, fill in the following fields:*

        1.  *In the VAT Bus. Posting Group field, remove the value EU and leave
            blank.*

    24. On the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter CHW1003.

        3.  In the **Location Code** field, the value EUROP is automatically
            filled in.

        4.  In the **Unit of Measure Code** field , the value PCS is
            automatically filled in.

        5.  In the **Quantity** field, enter ‘5’.

    25. Select **Posting** and then select **Post**.

    26. Select the **Ship** option and click **OK**.

    27. Close the **Sales Order** page.

2.  Use the Combine Shipments function to create sales invoices.

    1.  Open the **Combine Shipments** task.

    2.  In the **Posting Date** and **Document Date** field, enter 1/31/2022.

    3.  Select the **Calc. Inv. Discount** checkbox.

    4.  Select the **Post Invoices** checkbox.

    5.  In the **Sell-to Customer No.** filter, enter CWEB0001.

    6.  Click **OK**.

    7.  Click **OK**.
