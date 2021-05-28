---
lab:
    title: 'Lab: Configure Purchasing'
    module: 'Module 4: Configure Sales and Purchasing'
---

## Exercise 1: Complete the vendor card

### Scenario

As the functional consultant, you are collecting more information about the
purchase process, and more particularly about the vendors who you are purchasing
from and the conditions surrounding ordering and delivering of the purchased
items.

In order to supply the brand-new European warehouse and to deliver the computer
hardware items to the European customers, these items are purchased from
European wholesalers. Some of these vendors have different sales points
throughout the country.

Vendor Cronus Cardoxy Sales is Contoso’s main supplier for all computer hardware
items. They have different locations from where to order:

-   Computers and monitors need to be ordered at the following location:

    Nyborgvej 566, DK-5000 ODENSE C – contact: Hr. Allan Vinther-Wahl

-   Other computer accessories are sold from another location:

    Havnevej 6, DK-4600 KOGE – contact: Fr. Karen Friske

Cronus Cardoxy Sales guarantees to deliver all goods within 5 days, according to
the ‘cost and freight’ shipment method.

### Tasks

1.  Create an order address for the vendor

2.  Specify receiving information

### Steps

1.  Create an order address for the vendor

    1.  On the **Vendors** list page, select vendor Cronus Cardoxy Sales
        (V9002).

    2.  To open the vendor card, select **Manage** and then select **Edit**.

    3.  In the vendor card, select **Related**, then select **Vendor** and then
        **Order Addresses**.

    4.  In the opened **Order Address List** page, select **+New**.

    5.  In the opened order address card, fill in the following fields:

        1.  In the **Code** field, enter COMP&MON

        2.  In the **Name** field, the value ‘Cronus Cardoxy Sales’ is
            automatically filled in.

        3.  In the **Address** field, enter ‘Nyborgvej 566’.

        4.  In the **City** field, enter ‘ODENSE C’.

        5.  In the **ZIP Code** field, the value ‘DK-5000’ is automatically
            filled in.

        6.  In the **Country/Region Code** field, the value ‘DK’ is
            automatically filled in.

        7.  In the **Contact** field, enter Hr. Allan Vinther-Wahl.

    6.  Close the order address card.

    7.  In the opened **Order Address List** page, select **+New**.

    8.  In the opened order address card, fill in the following fields:

        1.  In the **Code** field, enter ACCESSORIE

        2.  In the **Name** field, the value ‘Cronus Cardoxy Sales’ is
            automatically filled in.

        3.  In the **Address** field, enter ‘Havnevej 6’.

        4.  In the **City** field, enter ‘KOGE’.

        5.  In the **ZIP Code** field, the value ‘DK-4600’ is automatically
            filled in.

        6.  In the **Country/Region Code** field, the value ‘DK’ is
            automatically filled in.

        7.  In the **Contact** field, enter Fr. Karen Friske.

    9.  Close the order address card.

    10. Close the **Order Address List** page.

2.  Specify receiving information

    1.  On the vendor card for vendor Cronus Cardoxy Sales, go to the
        **Receiving** FastTab.

    2.  In the **Location Code** field, enter EUROP.

    3.  In the **Shipment Method Code** field, enter CFR.

    4.  In the **Lead Time Calculation** field, enter 5D.

## Exercise 2: Complete the item card

### Scenario

The computer hardware items are not manufactured by Contoso, but purchased
through wholesalers, with Cronus Cardoxy Sales considered to be the main
supplier.

Cronus Cardoxy Sales guarantees to deliver all goods within 5 days, however some
special items may take a bit longer and have a deviating delivery time. For
example, the 17” monitor will take up to 7D to deliver.

All items can only be purchased in boxes, containing 10 pieces of the hardware.

You need to set up the replenishment information on the item card.

*Remark: For exercise purposes, only set up the catalog for the monitors.*

### Tasks

1.  Specify replenishment information

### Steps

1.  Specify replenishment information

    1.  On the **Items** list page, select item 15” 1501 FP Flat Panel (CHW1002)

    2.  To open the item card, select **Manage** and then select **Edit**.

    3.  In the item card, go to the **Replenishment** FastTab and fill in the
        following fields:

        1.  In the **Replenishment System** field, leave the default value
            **Purchase**.

        2.  In the **Lead Time Calculation** field, enter 5D.

        3.  In the **Vendor No.** field, enter V9002.

        4.  In the **Purch. Unit of Measure** field, the value PCS is already
            filled in. Click on the Look Up Value button and select **+New**.

        5.  In the opened **Item Units of Measure** page, fill in the following
            fields:

            1.  In the **Code** field, enter BOX.

            2.  In the **Qty. per Unit of Measure** field, enter 10.

        6.  Click **OK** to close the page.

        7.  The new code is automatically filled in in the **Purch. Unit of
            Measure** field on the item card.

    4.  Close the item card.

    5.  On the **Items** list page, select item 17" M780 Monitor (CHW1003)

    6.  To open the item card, select **Manage** and then select **Edit**.

    7.  In the item card, go to the **Replenishment** FastTab and fill in the
        following fields:

        1.  In the **Replenishment System** field, leave the default value
            **Purchase**.

        2.  In the **Lead Time Calculation** field, enter 7D.

        3.  In the **Vendor No.** field, enter V9002.

        4.  In the **Purch. Unit of Measure** field, the value PCS is already
            filled in. Click on the Look Up Value button and select **+New**.

        5.  In the opened **Item Units of Measure** page, fill in the following
            fields:

            1.  In the **Code** field, enter BOX.

            2.  In the **Qty. per Unit of Measure** field, enter 10.

        6.  Click **OK** to close the page.

        7.  The new code is automatically filled in in the **Purch. Unit of
            Measure** field on the item card.

    8.  Close the item card.

## Exercise 3: Set up an item vendor catalog

### Scenario

Although Cronus Cardoxy Sales is considered the main supplier for all computer
hardware items, these products can also be purchased with other vendors. For
example, when the item is temporarily out of stock.

When replenishing the item, Contoso will use the requisition worksheet, where
the main supplier will be suggested. However, it must be possible to order from
other available suppliers as well. Purchase orders will be sent to the vendors,
based on the vendors item numbers.

You will set up an item vendor catalog for all computer hardware items, as
follows:

-   All items can be purchased with vendor Cronus Cardoxy Sales (V9002).

-   All monitors can be purchased with vendor Pure-Look (V9005) and can be
    provided within 2 days:

    -   PLM-345 = 15" 1501 FP Flat Panel

    -   PLM-346 = 17" M780 Monitor

-   All accessories can be purchased with vendor WoodMart Supply Co. (V9006) and
    can be provided within 10 days:

    -   WMSA-10035 = Advanced Mouse

    -   WMSA-10036 = Quietkey keyboard

    -   WMSA-10037 = Speakers

*Remark: For exercise purposes, only set up the catalog for the monitors.*

### Tasks

1.  Set up an item vendor catalog

### Steps

1.  Set up an item vendor catalog

    1.  On the **Items** list page, select item 15” 1501 FP Flat Panel (CHW1002)

    2.  To open the item card, select **Manage** and then select **Edit**.

    3.  In the item card, select **Related**, then select **Purchases** and then
        **Vendors**.

    4.  On the opened **Item Vendor Catalog** page, select **+New**.

    5.  On the new line, fill in the following fields:

        1.  In the **Vendor No.** field, enter V9005.

        2.  In the **Vendor Item No.** field, enter PLM-345.

        3.  In the **Lead Time Calculation** field, enter 2D.

    6.  Close the **Item Vendor Catalog** page.

    7.  Close the item card.

    8.  On the **Items** list page, select item 17" M780 Monitor (CHW1003)

    9.  To open the item card, select **Manage** and then select **Edit**.

    10. In the item card, select **Related**, then select **Purchases** and then
        **Vendors**.

    11. On the opened **Item Vendor Catalog** page, select **+New**.

    12. On the new line, fill in the following fields:

        1.  In the **Vendor No.** field, enter V9005.

        2.  In the **Vendor Item No.** field, enter PLM-346.

        3.  In the **Lead Time Calculation** field, enter 2D.

    13. Close the **Item Vendor Catalog** page.

    14. Close the item card.

## Exercise 4: Configure recurring purchase lines

### Scenario

Next to the suppliers of trading goods, Contoso also has a numerous amount of
other costs. Often on a monthly recurring basis, the same purchase invoices need
to be processed.

To reduce the processing time, you explain the configuration of ‘recurring
purchase lines’ and together with the accounting manager, you set up the
following example:

Contoso has to pay a ‘health& dental insurance’ for each employee at the
company. They receive a monthly invoice with a fixed amount. These costs need to
be processed per department, as follows:

-   The total amount of the invoice is CAD 1,200.00, which is processed on the
    610000 income statement account.

-   25% of the cost is for the sales department.

-   35% of the cost is for the administration department.

-   40% of the cost is for the production department.

You need to set up the recurring purchase lines for vendor OakvilleWorld
(V9007), so that these lines are automatically filled in when creating a new
purchase invoice.

### Tasks

1.  Configure recurring purchase lines

### Steps

1.  Configure recurring purchase lines

    1.  On the **Vendors** list page, select vendor Oakville World (V9007).

    2.  Select **Related**, then **Purchases** and then select **Recurring
        Purchase Lines**.

    3.  On the opened **Recurring Purchase Lines** page, select **+New**.

    4.  On the new line, fill in the following fields:

        1.  Click on the Look Up Value button in the **Code** field, and select
            **+New**.

        2.  On the opened **Standard Purchase Code Card** page, fill in the
            following fields:

            1.  In the **Code** field, enter INSURANCE

            2.  In the **Description** field, enter ‘Monthly health insurance’

            3.  In the **Currency Code** field, enter CAD.

            4.  In the **Lines** section, create a new line, and fill in the
                following fields:

                1.  In the **Type** field, select the ‘G/L Account’ option.

                2.  In the **No.** field, enter 61000.

                3.  In the **Quantity** field, enter 1.

                4.  In the Amount excl. Tax field, enter ‘300’. (25% of
                    1,200.00)

                5.  In the **Department Code** field, enter SALES.

            5.  In the **Lines** section, create a new line, and fill in the
                following fields:

                6.  In the **Type** field, select the ‘G/L Account’ option.

                7.  In the **No.** field, enter 61000.

                8.  In the **Quantity** field, enter 1.

                9.  In the Amount excl. Tax field, enter ‘420’. (35% of
                    1,200.00)

                10. In the **Department Code** field, enter ADM.

            6.  In the **Lines** section, create a new line, and fill in the
                following fields:

                11. In the **Type** field, select the ‘G/L Account’ option.

                12. In the **No.** field, enter 61000.

                13. In the **Quantity** field, enter 1.

                14. In the Amount excl. Tax field, enter ‘480’. (40% of
                    1,200.00)

                15. In the **Department Code** field, enter PROD.

            7.  Close the **Standard Purchase Code Card** page.

            8.  Click **OK** to close the **Recurring Purchase Lines** page.

        3.  The new code is now automatically filled in in the **Code** field on
            the **Recurring Purchase Lines** page.

        4.  In the **Insert Rec. Lines On Invoices** field, select the
            **Automatic** option.

    5.  Close the **Recurring Purchase Lines** page
