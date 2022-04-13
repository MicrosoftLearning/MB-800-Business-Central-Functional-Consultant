
---
lab:
    title: 'Lab: Configure Sales Pricing and Discounts'
    module: 'Module 4: Configure Sales and Purchasing'
---

Hands-on-Lab 4.2: Configure Sales Pricing and Discounts
=======================================================

Exercise 1: Configure sales pricing and discounts
-------------------------------------------------

### Scenario

The sales manager at Contoso, has determined the following rules regarding their
sales of computer hardware:

-   All sales prices are set in local currency (LCY), which is the USD.

-   For each item a general sales price for all EU customers is determined for
    the base unit of measure. However, when large amounts are ordered, a lower
    unit price is granted.

    -   The 15” flat panel is sold at LCY 499.95 a piece. However, if the
        customer orders a box of 10 pieces, the price is lowered to LCY 4,800.00
        for the entire box.

    -   The 17” monitor is sold at LCY 700.00 a piece, However, if the customer
        orders a box of 10 pieces, the price is lowered to LCY 6,550.00 for the
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
    the order for sales above LCY 50.00 .

You have to set up this sales price structure as provided by Contoso.

In order to setup the sales prices per box, make sure this unit of measure is
created for the monitors.

### Tasks

1.  Set up customer price groups

2.  Set up customer discount groups

3.  Assign customer price groups and customer discount groups

4.  Set up and assign item discount groups

5.  Configure item units of measure

6.  Configure sales prices

7.  Configure line discount

8.  Configure invoice discount

### Steps

1.  Set up customer price groups

    1.  On the **Customers Price Groups** page, select **New**.

    2.  On the new line, fill in the following fields:

        1.  In the **Code** field, enter EU.

        2.  In the **Description** field, enter ‘EU customers’.

        3.  Leave the **Allow Line Disc.** and **Allow Invoice Disc.**
            checkboxes selected.

    3.  Repeat steps a. and b. to create also a DOMESTIC and EXPORT customer
        price group.

2.  Set up customer discount groups

    1.  On the **Customer Disc. Groups** page, select **New**.

    2.  On the new line, fill in the following fields:

        1.  In the **Code** field, enter SMALL.

        2.  In the **Description** field, enter ‘Small business’.

    3.  Repeat steps a. and b. to create also a MEDIUM and LARGE customer
        discount group.

3.  Assign customer price groups and customer discount groups

    1.  On the **Customers** list page, select the web shop customer (CWEB0001).

    2.  To open the customer card, select **Manage** and then select **Edit**.

    3.  Go to the **Invoicing** FastTab, and fill in the following fields:

        1.  In the **Customer Price Group** field, enter EU.

        2.  In the **Customer Disc. Group** field, enter SMALL

        3.  Leave the **Allow Line Disc.** checkbox selected.

    4.  Repeat steps d. to f. to assign the DOMESTIC customer price group to the
        customers C00010, C00020 and C00030 , and the SMALL customer discount
        group to customer C00010, the MEDIUM customer discount group to customer
        C00020 and the LARGE customer discount group to customer C00030.

4.  Set up and assign item discount groups

    1.  On the **Item Discount Groups** page, select **New**.

    2.  On the new line, fill in the following fields:

        1.  In the **Code** field, enter COMPUTER

        2.  In the **Description** field, enter ‘Computer’

    3.  Repeat step a. and b. to create an item discount group for MONITOR and
        ACCESSORIES

    4.  On the **Items** list page, select the 15” Flat panel (CHW1002)

    5.  Go to the **Prices & Sales** FastTab, in the **Item Disc. Group** field,
        enter MONITOR.

    6.  On the **Items** list page, select the 17” Flat panel (CHW1003)

    7.  Go to the **Prices & Sales** FastTab, in the **Item Disc. Group** field,
        enter MONITOR.

5.  Configure item units of measure

    1.  On the **Items** list page, select the 15” Flat panel (CHW1002).

    2.  To open the item card, select **Manage** and then select **Edit**.

    3.  On the opened item card, select **Related**, then select **Item** and
        then **Units of Measure**.

    4.  In the opened **Item Units of Measure** page, select **New** and fill in
        the following fields:

        1.  In the **Code** field, enter BOX

        2.  In the **Qty. per Unit of Measure** field, enter 10.

    5.  Click **OK** to close the page.

    6.  Close the item card.

    7.  Repeat steps a. to f. for the 17” Flat panel (CHW1003).

6.  Configure sales prices

    1.  On the **Items** list page, select the 15” flat panel (CHW1002).

    2.  To open the item card, select **Manage** and then select **Edit**.

    3.  On the opened item card, select **Prices & Discounts** and then select
        **Sales Prices**.

    4.  On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter Customer Price Group.

        2.  In the **Sales Code** field, enter EU.

        3.  In the **Item No**. field, the value CHW1002 is automatically filled
            in.

        4.  In the **Unit of Measure Code** field, the value PCS is
            automatically filled in.

        5.  In the **Unit Price** field, enter 499.95.

    5.  On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter Customer Price Group.

        2.  In the **Sales Code** field, enter EU.

        3.  In the **Item No**. field, the value CHW1002 is automatically filled
            in.

        4.  In the **Unit of Measure Code** field, the value PCS is
            automatically filled in. Change the value to BOX.

        5.  In the **Unit Price** field, enter 4800.00.

    6.  Close the sales prices page.

    7.  Close the item card.

    8.  On the Items list page, select the 17” monitor (CHW1003).

    9.  To open the item card, select **Manage** and then select **Edit**.

    10. On the opened item card, select **Prices & Discounts** and then select
        **Sales Prices**.

    11. On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter ‘Customer Price Group’.

        2.  In the **Sales Code** field, enter EU.

        3.  In the **Item No**. field, the value CHW1003 is automatically filled
            in.

        4.  In the **Unit of Measure Code** field, the value PCS is
            automatically filled in.

        5.  In the **Unit Price** field, enter 700.00.

    12. On the **Sales Prices** page, create a new line as follows:

        1.  In the **Sales Type** field enter Customer Price Group.

        2.  In the **Sales Code** field, enter EU.

        3.  In the **Item No**. field, the value CHW1003 is automatically filled
            in.

        4.  In the **Unit of Measure Code** field, the value PCS is
            automatically filled in. Change the value to BOX.

        5.  In the **Unit Price** field, enter 6,550.00.

7.  Configure line discount

    1.  On the **Item Discount Groups** page, make sure the item discount group
        for monitors is selected.

    2.  Select **Prices & Discounts** and then select **Sales Lines Discounts**.

    3.  On the **Sales Discounts** page, the **Type Filter** and **Code Filter**
        filters are automatically filled in.

    4.  Create a new line as follows:

        1.  In the **Sales Type** field enter Customer Disc. Group.

        2.  In the **Sales Code** field, enter SMALL.

        3.  In the **Type** field, enter Item Discount Group

        4.  In the **Code** field, enter MONITOR.

        5.  In the **Line Discount %** field, enter ‘3’.

    5. On the **Sales Line Discounts** page, create a new line as follows:

        1.  In the **Sales Type** field enter Customer Disc. Group.

        2.  In the **Sales Code** field, enter MEDIUM.

        3.  In the **Type** field, enter Item Discount Group

        4.  In the **Code** field, enter MONITOR.

        5.  In the **Line Discount %** field, enter ‘6’.

    6. On the **Sales Line Discounts** page, create a new line as follows:

        1.  In the **Sales Type** field enter Customer Disc. Group.

        2.  In the **Sales Code** field, enter LARGE.

        3.  In the **Type** field, enter Item Discount Group

        4.  In the **Code** field, enter MONITOR.

        5.  In the **Line Discount %** field, enter ‘10’.

    7.  Close the **Sales Line Discounts** page.

8.  Configure invoice discount

    1.  On the **Customers** list page, select the web shop customer (CWEB0001)

    2.  To open the customer card, select **Manage** and then select **Edit**.

    3.  Select **Related**, then select **Prices & Discounts** and then select
        **Invoice Discounts**.

    4.  On a new line, fill in the following fields.

        1.  In the **Minimum Amount** field, enter 50.00.

        2.  In the **Discount %** field, enter 5.

    5.  Close the **Cust. Invoice Discounts** page.
