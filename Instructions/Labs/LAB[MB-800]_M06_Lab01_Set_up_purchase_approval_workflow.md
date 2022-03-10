
---
lab:
    title: 'Lab: Order Promising'
    module: 'Module 5: Operations'
---

Hands-on-Lab 5.3: Order Promising
=================================

Exercise 1: Complete setup regarding order promising
----------------------------------------------------

### Scenario

When selling their webshop items to the European market, Contoso would like to
indicate the delivery date to the customers. Therefor the following date
calculations need to be set up:

-   The European warehouse generally needs about 1 day to pick, pack and label
    the items before shipping them to the customer.

-   Shipping is handled through the shipping agent DHL who standard guarantees a
    maximum delivery time within 2 days.

-   Both Contoso and DHL have a weekly closing day on Sunday.

### Tasks

1.  Setup a base calendar.

2.  Date calculation setup for sales orders.

### Steps

1.  Setup a base calendar

    1.  On the **Base Calendars** page, select **New**.

    2.  On the base calendar card, fill in the following fields:

        1.  In the **Code** field, enter BASE.

        2.  In the **Name** field, enter ‘Base Calendar’.

    3.  Select **Actions**, then select **Functions** and then select **Maintain
        Base Calendar Changes**.

    4.  On the **Base Calendar Changes** page, select **New**.

    5.  On the new line, fill in the following fields:

        1.  In the **Recurring System** field, enter ‘Weekly Recurring’.

        2.  In the **Day** field, enter ‘Sunday’.

        3.  In the **Description** field, enter ‘closing day’.

        4.  Select the **Nonworking** checkbox.

    6.  Close the **Base Calendar Changes** page.

2.  Date calculation setup for sales orders.

    1.  On the **Locations** list page, select the European warehouse (EUROP).

    2.  To open the location card, select **Manage** and then select **Edit**.

    3.  In the location card, go to the **Warehouse** FastTab.

        1.  In the **Outbound Whse. Handling Time** field, enter 1D.

        2.  In the **Base Calendar Code** field, enter BASE.

    4.  Close the **Location Card** page.

    5.  On the **Shipping Agents** list page, select DHL.

    6.  Select **Related**, then select **Line** and then **Shipping Agent
        Services**.

    7.  On the **Shipping Agent Services** page, select the line for the
        standard delivery service, which is already set up.

        1.  Confirm that the **Shipping Time** field contains a value of ‘2D’.

        2.  In the **Base Calendar Code** field, enter BASE.

    8.  Close the **Shipping Agent Services** page.

Exercise 2: Complete setup regarding requisition 
-------------------------------------------------

### Scenario

Contoso is not a manufacturer, so in order to replenish the European warehouse,
all items will be purchased. They will be using a requisition worksheet to
establish all necessary purchase orders.

More particularly the computer accessories will be handled as follows:

-   The main vendor for these items is WoodMart Supply Co. (V9006), a vendor
    from the UK.

-   WoodMart Supply Co. has the following items available:

    -   WMSA-10035 = Advanced Mouse

    -   WMSA-10036 = Quietkey keyboard

    -   WMSA-10037 = Speakers

-   Delivery time for these computer accessories is set to 10 working days.

-   The European warehouse needs about 1 day to handle the purchase receipts.

-   WoodMart has a closing day on Sunday.

These items will not be kept in inventory, but will only be purchased based on
sales orders. The requisition worksheet will be filled by using the capable to
promise functionality on the sales orders.

### Tasks

1.  Complete item replenishment.

2.  Date calculation setup.

3.  Setup Order Promising setup

### Steps

1.  Complete item replenishment

    1.  On the **Items** list page, select item Advanced Mouse (CHW1004)

    2.  To open the item card, select **Manage** and then select **Edit**.

    3.  In the item card, go to the **Replenishment** FastTab.

        1.  In the **Replenishment System** field, enter ‘Purchase’.

        2.  In the **Lead Time Calculation** field, enter 10D

        3.  In the **Vendor No.** field, enter V9006.

        4.  In the **Vendor Item No.** field, enter WMSA-10035

    4.  In the item card, go to the **Planning** FastTab

        1.  In the **Reordering Policy** field, enter ‘Order’.

    5.  Repeat steps a. to d. for items CHW1005 en CHW1006.

2.  Date calculation setup.

    1.  On the **Locations** list page, select the European warehouse (EUROP).

    2.  To open the location card, select **Manage** and then select **Edit**.

    3.  In the location card, go to the **Warehouse** FastTab.

        1.  In the **Inbound Whse. Handling Time** field, enter 1D.

    4.  Close the **Location Card** page.

3.  Setup Order Promising setup

    1.  On the **Order Promising Setup** page, make the following changes:

        1.  In the **Order Promising Template** field, enter the requisition
            worksheet REQ.

        2.  In the **Order Promising Worksheet** field, leave the DEFAULT value.

Exercise 3: Use the promise delivery dates on a sales order 
------------------------------------------------------------

### Scenario

On January 15th, 2022 a sales order was placed on the webshop by customer
Francematic for 10 Quietkey keyboards at LCY 54.50 a piece.

This customer will thus be serviced through the European warehouse and shipped
to the customer using DHL standard delivery services. Francematic requested for
the items to be delivered on January 20th, 2022.

Since computer accessories are not kept in stock, a purchase order must be
generated and the a promised delivery date must calculated.

### Tasks

1.  Create a sales order with a requested delivery date.

2.  Use order promising on the sales order.

### Steps

1.  Create a sales order with a requested delivery date.

    1.  On the **Sales Orders** list page, select **New**.

    2.  On the **General** FastTab, fill in the following fields:

        1.  In the **Customer No.** field, enter C00040.

        2.  In the **Order Date** field, enter 1/15/2022.

        3.  In the **Requested Delivery Date** field, enter 1/20/2022.

    3.  On the **Shipping and Billing** FastTab, fill in the following fields:

        1.  In the **Agent** field, enter DHL.

        2.  In the **Agent Service** field, enter STANDARD.

        3.  The **Shipping Time** field is now automatically filled in with 2D.

        4.  In the **Location Code** field, enter EUROP.

        5.  The **Outbound Whse. Handling Time** field is now automatically
            filled in with 1D.

    4.  In the **Lines** section, enter a new line by filling in the following
        fields:

        1.  In the **Type** field, enter Item.

        2.  In the **No.** field, enter CHW1005.

        3.  You will get a warning that the requested delivery date can not be
            met.

        4.  Click **OK**.

        5.  In the **Location Code** field, the value EUROP is automatically
            filled in.

        6.  In the **Unit of Measure Code** field, the value PCS is
            automatically filled in.

        7.  In the **Quantity** field, enter ‘10’.

        8.  In the **Unit Price excl. Tax** field, enter 54.50.

        9.  In the **Shipment Date** field, a date of 1/17/2022 is calculated.

        10. In the **Planned Shipment Date** field, a date of 1/18/2022 is
            calculated.

        11. In the **Planned Delivery Date** field, a date of 1/20/2022 is
            filled in, based on the requested delivery date.

    5.  A notification appears that the available inventory is to low.

2.  Use order promising on the sales order.

    1.  On the created sales order, select **More options**, select **Actions**, then select **Plan** and
        then **Order Promising**.

    2.  In the **Availability** field, you will see a value of -10.

    3.  Select **Capable-to-Promise**.

    4.  The **Earliest Shipment Date** field is calculated as 1/19/2022.

    5.  Select **Accept**.

    6.  Close the **Order Promising** page.

    7.  On the sales order, go to the **General** FastTab.

    8.  In the **Promised Delivery Date** field, enter 1/20/2022.

    9.  Click **Yes** to update the lines.
