---
lab:
    title: 'Lab: Configure Sales'
    module: 'Module 4: Configure Sales and Purchasing'
---

Hands-on-Lab 4.3: Configure Sales
=================================

Exercise 1: Complete the customer card
--------------------------------------

### Scenario

As the functional consultant, you are collecting more information about the
sales process, and more particularly about the customers who are buying your
products and the conditions surrounding delivery.

To deliver the computer hardware items from the European warehouse to the
European customers, Contoso uses DHL as a shipping agent. Web shop customers who
are end-users will have the option to choose between home delivery or delivery
at a pick-up point.

The following different pick-up points are set up as shipping addresses on the
Generic EU web shop customer (CWEB0001):

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

In the domestic areas, sales activities are performed by sales representatives
who each have their set of customers. All transactions need to be assigned to a
specific salesperson as follows:

-   C00010 Spotsmeyer’s Furnishings is a customer from Annette Hill

-   C00020 Progressive Home Furnishings is a customer from John Roberts

-   C00030 New Concepts Furniture is a customer from Peter Saddow

Also don’t forget to assign de SALESPERSON dimension to each salesperson.

### Tasks

1.  Create a shipping address for the customer.

2.  Specify shipping information.

3.  Set up and assign a salesperson

### Steps

1.  Create a shipping address for the customer.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Customers**, and then choose the related link.

    2.  On the **Customers** list page, select the **Generic EU web shop
        (CWEB0001)**.

    3.  To open the customer card, select **Manage** and then select **Edit**.

    4.  In the customer card, select **Related**, then select **Customer** and
        then **Ship-to Addresses**.

    5.  In the opened **Ship-to Address** List page, select **+ New**.

    6.  In the opened ship-to addresses card, fill in the following fields:

        1.  In the **Code** field, enter **PICK-UP DK**

        2.  In the **Name** field, the value **Generic EU web shop** is
            automatically filled in. Replace with **Pick-up point Denmark**.

        3.  In the **Address** field, enter **Carl Blochs Gade 7**.

        4.  In the **City** field, enter **Arhus C**

        5.  In the **ZIP Code** field, the value **DK-8000** is automatically
            filled in.

        6.  In the **Country/Region Code** field, the value **DK** is
            automatically filled in.

        7.  In the **Contact** field, enter **Hr. Jonathan Mollerup**.

    7.  Close the ship-to address card.

    8.  In the customer card, select **Related**, then select **Customer** and
        then **Ship-to Addresses**.

    9.  In the opened **Ship-to Address List** page, select **+ New**.

    10. In the opened ship-to addresses card, fill in the following fields:

        1.  In the **Code** field, enter **PICK-UP BE**

        2.  In the **Name** field, the value **Generic EU web shop** is
            automatically filled in. Replace with **Pick-up point Belgium**.

        3.  In the **Address** field, enter **Binkkampen 33**.

        4.  In the **City** field, enter **Brussel**

        5.  In the **ZIP Code** field, enter **BE-1020**.

        6.  In the **Country/Region Code** field, the value **BE** is
            automatically filled in.

        7.  In the **Contact** field, enter **Caroline Pedersen**.

    11. Close the ship-to address card.

    12. In the customer card, select **Related**, then select **Customer** and
        then **Ship-to Addresses**.

    13. In the opened **Ship-to Address** List page, select **+ New**.

    14. In the opened ship-to addresses card, fill in the following fields:

        1.  In the **Code** field, enter **PICK-UP FR**

        2.  In the **Name** field, the value **Generic EU web shop** is
            automatically filled in. Replace with **Pick-up point France**.

        3.  In the **Address** field, enter **34 Avenue Parmentier**.

        4.  In the **City** field, enter **Paris**

        5.  In the **ZIP Code** field, the value **FR-75000** is automatically
            filled in.

        6.  In the **Country/Region Code** field, the value **FR** is
            automatically filled in.

        7.  In the **Contact** field, enter **M. Jean E. TRENARY**.

    15. Close the ship-to address card.

    16. Close the **Ship-to Address List** page.

2.  Specify shipping information.

    1.  On the customer card for the **Generic EU Web Shop** Customer
        **(CWEB0001)**, go to the **Shipping** FastTab.

    2.  Leave the **Ship-to Code** field blank.

    3.  In the **Location Code** field, enter **EUROP**.

    4.  Click **Show more**.

    5.  In the **Agent** field, enter **DHL**

    6.  In the **Agent Service** field, enter **STANDARD**

    7.  In the **Shipping Time** field, the value **2D** is automatically filled
        in.

3.  Set up and assign a salesperson

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Sales People/Purchasers**, and then choose the related link.

    2.  On the **Sales People/Purchasers** list page, select **+ New**.

    3.  In the **Code** field, enter **AH** and in the **Name** field enter
        **Annette Hill**.

    4.  Close the Salesperson/Purchaser card.

    5.  On the **Salespeople/Purchaser** page, make sure that you have selected
        **Annette Hill**. Click on **Salesperson** and then select
        **Dimensions-single** from the dropdown.

    6.  On the opened **Default Dimensions** page, select **+ New**.

    7.  On the new line, fill in the following fields:

        1.  In the **Dimension Code** field, enter **SALESPERSON_NEWLIST**

        2.  In the **Dimension Value Code** field, enter **AH**

        3.  In the **Value Posting** field, select the **Same Code** option.

        4.  Close the page.

    8.  Repeat steps b. to g. for salespeople **John Roberts** and **Peter
        Saddow**.

        *(Remark: you also repeat the steps for the other salespeople, but this
        is not required for further exercises.)*

    9.  Select the search for page icon in the top-right corner of the page,
        enter **Customers**, and then choose the related link.

    10. On the **Customers** list page, select **Trey Research (20000)**.

    11. To open the customer card, select **Manage** and then select **Edit**.

    12. On the **General** FastTab, in the **Salesperson Code** field, enter
        **AH**

    13. Go to the next customer card for customer **Relecloud (50000)**.

    14. On the **General** FastTab, in the **Salesperson Code** field, enter
        **JR**

    15. Go to the next customer card for customer **School of Fine Art
        (30000)**.

    16. On the **General** FastTab, in the **Salesperson Code** field, enter
        **PS**

Exercise 2: Configure sales pricing and discounts
-------------------------------------------------

### Scenario

The sales manager at Contoso, has determined the following rules regarding their
sales of computer hardware:

-   All sales prices are set in local currency, thus USD.

-   For each item, a general sales price for all EU customers is determined for
    the base unit of measure. However, when large amounts are ordered, a lower
    unit price is granted.

    -   The 15” flat panel is sold at \$ 499.95 per piece. However, if the
        customer orders a box of 10 pieces, the price is lowered to \$ 4,800.00
        for the entire box.

    -   The 17” monitor is sold at \$ 700.00 a piece, However, if the customer
        orders a box of 10 pieces, the price is lowered to \$ 6,550.00 for the
        entire box.

    -   For other customers (both domestic and non-EU) separate sales prices
        will be determined later.

-   Depending on the customer group (small, medium, large) and item group
    (computer, monitor, accessories) a discount percentage is granted to achieve
    the net sales price.

    -   The generic web shop customer and all other small businesses receive a
        standard 3% on all monitors. Medium sized customers receive 6% and large
        companies receive 10% on the same items.

-   To boost web shop sales, a discount of 5% is granted on the total amount of
    the order for sales above \$50.00 .

You must set up this sales price structure as provided by Contoso.

### Tasks

1.  Set up customer price groups

2.  Set up customer discount groups

3.  Assign customer price groups and customer discount groups

4.  Set up and assign item discount groups

5.  Configure sales prices

6.  Configure line discount

7.  Configure invoice discount

### Steps

1.  Set up customer price groups

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Customers Price Groups**, and then choose the related link.

    2.  On the **Customers Price Groups** page, select **+ New**.

    3.  On the new line, fill in the following fields:

        1.  In the **Code** field, enter **EU**.

        2.  In the **Description** field, enter **EU customers**.

        3.  Leave the **Allow Line Disc.** and **Allow Invoice Disc.**
            checkboxes selected.

    4.  Repeat steps a. and b. to create also a **DOMESTIC** and **EXPORT**
        customer price group.

2.  Set up customer discount groups

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Customer Disc. Groups**, and then choose the related link.

    2.  On the **Customer Disc. Groups** page, select **+ New**.

    3.  On the new line, fill in the following fields:

        1.  In the **Code** field, enter **SMALL**.

        2.  In the **Description** field, enter **Small business**.

    4.  Repeat steps a. and b. to create also a **MEDIUM** and **LARGE**
        customer discount group.

3.  Assign customer price groups and customer discount groups

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Customer**, and then choose the related link.

    2.  On the **Customers** list page, select the **Generic EU Web Shop**
        Customer **(CWEB0001)**.

    3.  To open the customer card, select **Manage** and then select **Edit**.

    4.  Go to the **Invoicing** FastTab, click **Show more** and fill in the
        following fields:

        1.  In the **Customer Price Group** field, enter **EU**.

        2.  In the **Customer Disc. Group** field, enter **SMALL**

        3.  Leave the **Allow Line Disc.** checkbox selected.

    5.  Repeat steps d. to f. to assign the **DOMESTIC** customer price group to
        the customers **20000**, **30000** and **50000**, and the **SMALL**
        customer discount group to customer **20000**, the **MEDIUM** customer
        discount group to customer **30000** and the **LARGE** customer discount
        group to customer **50000**.

4.  Set up and assign item discount groups

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Item Discount Groups**, and then choose the related link.

    2.  On the **Item Discount Groups** page, select **+ New**.

    3.  On the new line, fill in the following fields:

        1.  In the **Code** field, enter **COMPUTER**

        2.  In the **Description** field, enter **Computer**

    4.  Repeat step b. and c. to create an item discount group for **MONITOR**
        and **ACCESSORIES**

    5.  Select the search for page icon in the top-right corner of the page,
        enter **Items**, and then choose the related link.

    6.  On the **Items** list page, select the **15” Flat panel (CHW1002)**

    7.  Go to the **Prices & Sales** FastTab, click **Show more**.

    8.  In the **Item Disc. Group** field, enter **MONITOR**.

    9.  On the **Items** list page, select the **17” M780 (CHW1002)**

    10. Go to the **Invoicing** FastTab, in the **Item Disc. Group** field,
        enter **MONITOR**.

5.  Configure sales prices

    1.  On the **Items** list page, select the **15” flat panel (CHW1002)**.

    2.  To open the item card, select **Manage** and then select **Edit**.

    3.  On the opened item card, select **Sales Prices & Discounts** and then
        select **Sales Prices**.

    4.  On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter **Customer Price Group**.

        2.  In the **Sales Code** field, enter **EU**.

        3.  In the **Item No**. field, the value **CHW1002** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value **PCS** is
            automatically filled in.

        5.  In the **Unit Price** field, enter **499.95**.

    5.  On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter **Customer Price Group**.

        2.  In the **Sales Code** field, enter **EU**.

        3.  In the **Item No**. field, the value **CHW1002** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value **PCS** is
            automatically filled in. Change the value to **BOX**.

        5.  In the **Unit Price** field, enter **4800.00**.

    6.  Close the sales prices page.

    7.  Close the item card.

    8.  On the Items list page, select the **17” monitor (CHW1003)**.

    9.  To open the item card, select **Manage** and then select **Edit**.

    10. On the opened item card, select **Sales Prices & Discounts** and then
        select **Sales Prices**.

    11. On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter **Customer Price Group**.

        2.  In the **Sales Code** field, enter **EU**.

        3.  In the **Item No**. field, the value **CHW1003** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value **PCS** is
            automatically filled in.

        5.  In the **Unit Price** field, enter **700.00**.

    12. On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter **Customer Price Group**.

        2.  In the **Sales Code** field, enter **EU**.

        3.  In the **Item No**. field, the value **CHW1003** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value **PCS** is
            automatically filled in. Change the value to **BOX**.

        5.  In the **Unit Price** field, enter **6,550.00**.

6.  Configure line discount

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Item Discount Groups**, and then choose the related link.

    2.  On the **Prices & Discounts** page, select **Sales Lines Discounts**.

    3.  Remove the value in the **Code Filter** filter.

    4.  On the **Sales Discounts** page, create a new line as follows:

        1.  In the **Sales Type** field enter **Customer Disc. Group**.

        2.  In the **Sales Code** field, enter **SMALL**.

        3.  In the **Type** field, enter **Item Discount Group**

        4.  In the **Code** field, enter **MONITOR**.

        5.  In the **Line Discount %** field, enter **3**.

    5.  On the **Sales Discounts** page, create a new line as follows:

        1.  In the **Sales Type** field enter **Customer Disc. Group**.

        2.  In the **Sales Code** field, enter **MEDIUM**.

        3.  In the **Type** field, enter **Item Discount Group**

        4.  In the **Code** field, enter **MONITOR**.

        5.  In the **Line Discount %** field, enter **6**.

    6.  On the **Sales Discounts** page, create a new line as follows:

        1.  In the **Sales Type** field enter **Customer Disc. Group**.

        2.  In the **Sales Code** field, enter **LARGE**.

        3.  In the **Type** field, enter **Item Discount Group**

        4.  In the **Code** field, enter **MONITOR**.

        5.  In the **Line Discount %** field, enter **10**.

    7.  Close the **Sales Discounts** page.

7.  Configure invoice discount

    1.  Select the search for page icon in the top-right corner of the page,
        **Customers**, and then choose the related link.

    2.  On the **Customers** page, select the **Generic EU Web Shop** Customer
        **(CWEB0001)**

    3.  To open the customer card, select **Manage** and then select **Edit**.

    4.  Select **Related**, then select **Prices and Discounts** and then select
        **Invoice Discounts**.

    5.  On a new line, fill in the following fields.

        1.  In the **Minimum Amount** field, enter **50.00**.

        2.  In the **Discount %** field, enter **5**.

    6.  Close the **Cust. Invoice Discounts** page.

