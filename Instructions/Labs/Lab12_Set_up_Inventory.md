Exercise 12: Set up Inventory 
==============================

Task 1: Configure the Inventory Setup
-------------------------------------

### Scenario

Concerning the processing of inventory-related transactions and the inventory
valuation, Contoso’s account manager has expressed the following requirements:

-   The web shop items for computer hardware are numbered separately from other
    items. They are incremented by 1, starting from the number CHW1000.

-   All items should be always tracked across the different warehouses.

-   Inventory value should be visible in the g/l balance accounts at each
    invoice/credit memo posting, while interim values are not registered.

-   To improve the inventory value process, negative inventory must be
    prohibited.

You will perform

1.  Set up and assign number series.

2.  Complete inventory costing setup.

3.  Make location mandatory and prevent negative inventory.

### Steps

1.  Set up and assign number series.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Inventory Setup**, and then choose the related link.

    2.  In the **Inventory Setup** page, go to the **Numbering** FastTab.

    3.  In the **Item Nos.** field, the value **ITEM** is already filled in.
        Click on the Look Up Value button and select **+ New**.

    4.  In the opened **No. Series List** page, fill in the following fields:

        1.  In the **Code** field, enter **COMPHW**

        2.  In the **Description** field, enter **Computer Hardware**.

        3.  Select the **Default Nos.** check box.

    5.  Click on the Lookup again and Click on View Details. Click the ellipses
        (…), select **Navigate** and then select **Lines**.

    6.  In the opened **No. Series Lines** page, select **+ New**.

        1.  Leave the **Starting Date** field blank.

        2.  In the **Starting No.** field, enter **CHW1000**.

        3.  In the **Increment-by No.** field, enter the value **1**.

    7.  Close the **No. Series Lines** page.

    8.  In the opened **No. Series List** page, select the number series
        **ITEM**.

    9.  Click the ellipses (…), select **Navigate** and then select
        **Relationships**.

    10. In the **No. Series Relationships** page, select **+ New**.

    11. In the **Series Code** field, enter **COMPHW**.

    12. Close the **No. Series Relationships** page.

    13. Close the **No. Series List** page by clicking **OK**.

    14. The number series **ITEM** remains filled in in the **Item Nos.** field,
        in the **Inventory Setup** page.

2.  Complete inventory costing setup.

    1.  In the **Inventory Setup** page, go to the **General** FastTab.

    2.  Click **Show more**.

    3.  Select the **Automatic Cost Posting** checkbox.

    4.  Deselect the **Expected Cost Posting to G/L** checkbox.

    5.  In the **Automatic Cost Adjustment** field, leave the **Always** option
        selected.

3.  Make location mandatory and prevent negative inventory.

    1.  In the **Inventory Setup** page, go to the **General** FastTab.

    2.  Select the **Prevent Negative Inventory** checkbox.

    3.  In the **Location** FastTab, select the **Location Mandatory** checkbox.

Task 2: Create and configure items
----------------------------------

### Scenario

For the sales of computer hardware items, Contoso has invested in a new
warehouse located in Europe. This warehouse contains only computer hardware, and
none of the other resale items. No warehouse tasks are required.

Also, in the chart of accounts the inventory value is registered separately on
the balance sheet account 10710, and the income statement account 50150.

You need to set up a new inventory posting group COMPHW and make sure the
general posting setup is configured correctly.

So far, only a few computer hardware items have been set up. These will be
created manually.

Different item features, such as inch, processor, color, will be registered as
additional information on the item cards. More specifically the following
computer hardware items are created:

You need to set up new item categories and configure the correct attributes.

Then you can manually enter the computer hardware items, using a configuration
template.

You will perform

1.  Create a location.

2.  Set up an Inventory Posting Group and complete the Inventory Posting Setup.

3.  Set up Item Categories and Item Attributes.

4.  Create and configure a new item.

### Steps

1.  Create a location.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Locations**, and then choose the related link.

    2.  In the **Locations** page, select **+New**

    3.  In the **Location Card** page, on the **General** FastTab, fill in the
        following fields:

        1.  In the **Code** field, enter **EUROP**.

        2.  In the **Name** field, enter **European warehouse**.

    4.  On the **Warehouse** FastTab, leave all the checkboxes deselected.

2.  Set up an Inventory Posting Setup.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Inventory Posting Groups**, and then choose the related link.

    2.  In the **Inventory Posting Groups** page, select **+ New**.

    3.  In the **Code** field, enter **COMPHW**.

    4.  In the **Description** field, enter **Computer Hardware**

    5.  Select **Setup**.

    6.  In the opened **Inventory Posting Setup** page, select **+ New**.

    7.  In the opened **Inventory Posting Setup Card** page, fill in the
        following fields:

        1.  In the **Location Code** field, enter **EUROP**.

        2.  The **Invt. Posting Group Code** field is automatically filled in
            with **COMPHW**.

        3.  In the **Inventory Account** field, enter **10710**.

    8.  Close the **Inventory Posting Setup Card**.

    9.  Select the search for page icon in the top-right corner of the page,
        enter **General Posting Setup**, and then choose the related link.

    10. In the **General Posting Setup** page, for each combination where the
        **Gen. Prod. Posting Group** field contains the value **COMPUTERHW**,
        make sure the following fields are filled in:

        1.  In the **COGS Account** field, enter **50150**.

        2.  In the **Inventory Adjmt. Account** field, enter **50150**.

        3.  In the **Direct Cost Applied Account** field, enter **50150**.

        4.  In the **Overhead Applied Account** field, enter **50150**.

3.  Set up Item Categories and Item Attributes.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Item Categories**, and then choose the related link.

    2.  In the **Item Categories** page, select **+ New**.

    3.  In the opened **Item Category Card** page, fill in the following fields:

        1.  In the **Code** field, enter **COMPHW**.

        2.  In the **Description** field, enter **Computer hardware**.

        3.  In the **Attributes** section, enter a new line, filling in the
            following fields:

            1.  In the **Attribute** field, click on the Look Up Value button
                and click **Select from full list**.

            2.  In the opened **Item Attributes** page, select the **Color**
                attribute.

            3.  Click on the **Values** of **Color**.

                1.  In the opened **Item Attributes Value** page, click **+
                    New**.

                2.  In the **Value** field, enter **Grey**

                3.  Close the **Item Attributes Value** page.

            4.  Click **OK** to close the **Item Attributes** page.

            5.  The new code is automatically filled in in the **Attribute**
                field on the item category card.

        4.  Close the item category card.

    4.  In the **Item Categories** page, select **+ New**.

    5.  In the opened **Item Category Card** page, fill in the following fields:

        1.  In the **Code** field, enter **COMPUTER**.

        2.  In the **Description** field, enter **Computer**.

        3.  In the **Parent Category** field, enter **COMPHW**.

        4.  In the **Attributes** section, enter a new line, filling in the
            following fields:

            1.  In the **Attribute** field, click on the Look Up Value button
                and click **+ New**.

            2.  In the opened **Item Attributes** page, on the new line, fill in
                the following fields:

                4.  In the **Name** field, enter **Processor**.

                5.  In the **Type** field, select the **Text** option.

                6.  Make sure the new line is selected.

                7.  Click **OK** to close the page.

            3.  The new code is automatically filled in in the **Attribute**
                field on the item category card.

        5.  Close the item category card.

    6.  In the **Item Categories** page, select **+ New**.

    7.  In the opened **Item Category Card** page, fill in the following fields:

        1.  In the **Code** field, enter **MONITOR**.

        2.  In the **Description** field, enter **Monitor**.

        3.  In the **Parent Category** field, enter **COMPHW**.

        4.  In the **Attributes** section, enter a new line, filling in the
            following fields:

            1.  In the **Attribute** field, click on the Look Up Value button
                and click **+ New**.

            2.  In the opened **Item Attributes** page, on the new line, fill in
                the following fields:

                8.  In the **Name** field, enter **Inch**.

                9.  In the **Type** field, select the **Decimal** option.

                10. Make sure the new line is selected.

                11. Click **OK** to close the page.

            3.  The new code is automatically filled in in the **Attribute**
                field on the item category card.

        5.  Close the item category card.

    8.  In the **Item Categories** page, select **+ New**.

    9.  In the opened **Item Category Card** page, fill in the following fields:

        1.  In the **Code** field, enter **ACCESSORIES**.

        2.  In the **Description** field, enter **Computer accessories**.

        3.  In the **Parent Category** field, enter **COMPHW**.

        4.  Close the item category card.

4.  Create an Item template.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Item Templates**, and then choose the related link.

    2.  In the **Item Templates** page, select **+ New**.

    3.  In the **Item Template** page, fill in the following fields:

        1.  In the **Code** field, enter **COMPHW**

        2.  In the **Description** field, enter **Computer hardware**

        3.  In the **No. Series** field, enter **COMPHW**.

    4.  Then go to the **Cost & Posting** FastTab and fill in the following
        fields

        1.  In the **Gen. Prod. Posting Group** field, enter **COMPUTERHW**.

        2.  In the **Inventory Posting Group** field, enter **COMPHW**.

5.  Close the item template.

6.  Create and configure a new item.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Items**, and then choose the related link.

    2.  On the **Items** page, select **New** and +New

    3.  Select the template **Computer hardware** and click **OK**.

    4.  A new item card is created with number **CHW1000**.

    5.  On the **Item** FastTab, fill in the following fields:

        1.  In the **Description** field, enter **Computer III 533 MHz**.

        2.  In the **Item Category Code** field, enter **COMPUTER**.

        3.  The **Base Unit of Measure** field is filled in with the default
            value **PCS**.

    6.  On the **Item Attribute** FactBox in the right side, select **Edit**.

        1.  For the attribute **Color**, select the value **black**.

        2.  For the attribute **Processor**, enter the value **533 Mhz**.

        3.  Click **OK** to close the FactBox.

    7.  Close the item card.

    8.  On the **Items** page, select **+ New**.

    9.  Select the template **Computer hardware** and click **OK**.

    10. A new item card is created with number **CHW1001**.

    11. On the **Item** FastTab, fill in the following fields:

        1.  In the **Description** field enter **Computer III 600 MHz**.

        2.  In the **Item Category Code** field, enter **COMPUTER**.

        3.  The **Base Unit of Measure** field is filled in with the default
            value **PCS**.

    12. On the **Item Attribute** FactBox, select **Edit**.

        1.  For the attribute **Color**, select the value **black**.

        2.  For the attribute **Processor**, enter the value **600 Mhz**.

        3.  Click **OK** to close the FactBox.

    13. Close the item card.

    14. On the **Items** page, select **+ New**.

    15. Select the template **Computer hardware** and click **OK**.

    16. A new item card is created with number **CHW1002**.

    17. On the **Item** FastTab, fill in the following fields:

        1.  In the **Description** field, enter **15" 1501 FP Flat Panel**.

        2.  In the **Item Category Code** field, enter **MONITOR**.

        3.  The **Base Unit of Measure** field is filled in with the default
            value **PCS**.

    18. On the **Item Attribute** FactBox, select **Edit**.

        1.  For the attribute **Color**, select the value **black**.

        2.  For the attribute **Inch**, enter the value **15**.

        3.  Click **OK** to close the FactBox.

    19. Close the item card.

    20. On the **Items** page, select **+ New**.

    21. Select the template **Computer hardware** and click **OK**.

    22. A new item card is created with number **CHW1003**.

    23. On the **Item** FastTab, fill in the following fields:

        1.  In the **Description** field, enter **17" M780 Monitor**.

        2.  In the **Item Category Code** field, enter **MONITOR**.

        3.  The **Base Unit of Measure** field is filled in with the default
            value **PCS**.

    24. On the **Item Attribute** FactBox, select **Edit**.

        1.  For the attribute **Color**, select the value **black**.

        2.  For the attribute **Inch**, enter the value **17**.

        3.  Click **OK** to close the FactBox.

    25. Close the item card.

    26. On the **Items** page, select **+ New**.

    27. Select the template **Computer hardware** and click **OK**.

    28. A new item card is created with number **CHW1004**.

    29. On the **Item** FastTab, fill in the following fields:

        1.  In the **Description** field, enter **Advanced Mouse**.

        2.  In the **Item Category Code** field, enter **ACCESSORIES**.

        3.  The **Base Unit of Measure** field is filled in with the default
            value **PCS**.

    30. On the **Item Attribute** FactBox, select **Edit**.

        1.  For the attribute **Color**, select the value **grey**.

        2.  Click **OK** to close the FactBox.

    31. Close the item card.

    32. On the **Items** page, select **+ New**.

    33. Select the template **Computer hardware** and click **OK**.

    34. A new item card is created with number **CHW1005**.

    35. On the **Item** FastTab, fill in the following fields:

        1.  In the **Description** field, enter **Quietkey keyboard**.

        2.  In the **Item Category Code** field, enter **ACCESSORIES**.

        3.  The **Base Unit of Measure** field is filled in with the default
            value **PCS**.

    36. On the **Item Attribute** FactBox, select **Edit**.

        1.  For the attribute **Color**, select the value **grey**.

        2.  Click **OK** to close the FactBox.

    37. Close the item card.

    38. On the **Items** page, select **+ New**.

    39. Select the template **Computer hardware** and click **OK**.

    40. A new item card is created with number **CHW1006**.

    41. On the **Item** FastTab, fill in the following fields:

        1.  In the **Description** field, enter **Speakers**.

        2.  In the **Item Category Code** field, enter **ACCESSORIES**.

        3.  The **Base Unit of Measure** field is filled in with the default
            value **PCS**. Change the value to **BOX**.

    42. On the **Item Attribute** FactBox, select **Edit**.

        1.  For the attribute **Color**, select the value **white**.

        2.  Click **OK** to close the FactBox.

    43. Close the item card.
