---
lab:
    title: 'Lab 14: Process Purchase'
    module: 'Learning Path 4: Perform Business Central operations'
---

Exercise 14: Process Purchase
=============================

Task 1: Process a purchase from order to invoice and review the posted documents
--------------------------------------------------------------------------------

### Scenario

As the purchasing agent you are replenishing the stock for the European
warehouse. The computer monitors are currently low on stock and a purchase order
with their main vendor Robert Townes is placed on January 1st, 2023. It was
agreed to always invoice in USD instead of their currency (DKK) and a purchase
request is sent to the correct order address for the following items to be
delivered on January 5th, 2023:

-   100 pieces of the 15” flat panel at \$ 4,999.89 a box, containing 10 pieces.

-   50 pieces of the 17” monitor at \$ 5,348.56 a box, containing 10 pieces

The purchase request is confirmed by the vendor on January 8th, 2023, with order
confirmation OC15-479. They mention a delivery delay of a couple of days,
expecting to be able to deliver the entire order on January 12th, 2023.

Eventually the goods are delivered with delivery notes DN01-47 on January 16th,
2023, as follows:

-   11 boxes of the 15” flat panel – this is 1 box more than ordered

-   4 boxes of the 17” monitor – this is 1 box less than ordered

The purchase invoice with number 20-0747 is received by mail on January 20th,
2023, where a 5% discount is granted on the 15” monitors as a compensation for
the delivery delay. The invoice needs to be paid within 30 days.

You will perform-

1.  Change the currency code on the vendor.

2.  Create a purchase order.

3.  Receive items on the purchase order.

4.  Create a posted purchase invoice from the purchase order.

5.  Review the posted purchase receipt and invoice.

### Steps

1.  Change the currency code on the vendor.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Vendors`, and then choose the related link.

    2.  On the **Vendors** list page, select vendor **Robert Townes (V9002)**.

    3.  Select **Manage** and then select **Edit**.

    4.  On the opened vendor card, go to the **Invoicing** FastTab, and click
        **Show more**.

    5.  Leave the **Currency Code** field blank.

2.  Create a purchase order.

    1.  On the vendor card, select **New Document** and then select **Purchase
        Order**.

    2.  On the **General** FastTab, fill in the following fields:

        1.  In the **Document Date** and **Order Date** fields, enter
            **1/1/2023**.

        2.  In the **Alternate Vendor Address Code** field, enter **COMP&MON**.

        3.  In the **Vendor Order No.** field, enter **OC15-479**.

    3.  On the **Invoice Details** FastTab, click **Show more** and then fill in
        the following fields:

        1.  In the **Requested Receipt Date** field, enter **1/05/2023**.

        2.  In the **Promised Receipt Date** field, enter **1/12/2023**.

    4.  On the **Lines** section, enter a new line by filling in the following
        field:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1002** for the **15” flat panels**.

        3.  In the **Location Code** field, the value **EUROP** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value **BOX** is
            automatically filled in.

        5.  In the **Quantity** field, enter **10**.

        6.  In the **Direct Unit Cost Excl. Tax** field, enter **4,999.89**.

        7.  In the **Tax Group Code**, enter **NONTAXABLE**.

    5.  On the **Lines** section, enter a new line by filling in the following
        field:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1003** for the **17” flat panels**.

        3.  In the **Location Code** field, the value **EUROP** is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value **BOX** is
            automatically filled in.

        5.  In the **Quantity** field, enter **5**.

        6.  In the **Direct Unit Cost Excl. Tax** field, enter **5,348.56**.

        7.  In the **Tax Group Code**, enter **NONTAXABLE**.

    6.  Select **Release**.

3.  Receive items on the purchase order.

    1.  On the **General** FastTab, fill in the following fields:

        1.  In the **Posting Date** field, enter **1/16/2022**.

        2.  In the **Vendor Shipment No.** field, enter **DN01-47**.

    2.  On the **Lines** section, select the line for item **CHW1002**, and fill
        in the following fields:

        1.  In the **Over-Receipt Code** field, enter **OVERRCPT10**.

        2.  In the **Qty. to Receive** field, enter **11**.

    3.  On the **Lines** section, select the line for item **CHW1003**, and fill
        in the following fields:

        1.  In the **Qty. to Receive** field, enter **4**.

    4.  Select the dropdown of **Posting**, and then select **Post**.

    5.  Select the **Receive** option and click **OK**.

4.  Create a posted purchase invoice from the purchase order.

    1.  Select the dropdown of **Release**, and then select **Reopen**.

    2.  On the **General** FastTab, fill in the following fields:

        1.  In the **Posting Date** field, enter **1/18/2023**.

        2.  In the **Vendor Invoice No.** field, enter **20-0747**.

    3.  On the **Invoice Details** FastTab, in the **Payment Terms Code** field,
        enter **30 DAYS**.

    4.  On the **Lines** section, select the line for item **CHW1002**, and
        click on the **Settings** icon in the top-right corner.

    5.  Select **Personalize** to add the **Line Discount%** field.

    6.  Click **More** on the **Personalizing** ribbon.

    7.  Select the **Lines** area and click **+ Field** in the **Personalizing**
        ribbon.

    8.  An **Add field to page** pane will appear on the right side.

    9.  Select **Line Discount %** from the **Add Field to Page** pane and drag
        it to the right of **Quantity** column in the **Lines** area.

    10. fill in the following fields:

        1.  In the **Line Discount%** field, enter **5**.

    11. Select the dropdown next to **Posting**, and then select **Post**.

    12. Select the **Invoice** option and click **OK**.

5.  Review the posted purchase receipt and invoice.

    1.  Select **Order** and select **Receipts**.

    2.  On the **Posted Purchase Receipts** page, select **Find Entries**.

    3.  Select the line for **Item Ledger Entry** and select **Show Related
        Entries**.

    4.  Close the **Item Ledger Entries** page.

    5.  Close the **Find Entries** page.

    6.  On the **Purchase Order** page, select **Order** and then select
        **Invoices**.

    7.  On the **Posted Purchase Invoices** page, select **Find Entries**.

    8.  Select the line for **G/L entries** and select **Show Related Entries**.

    9.  Close the **General Ledger Entries** page.

    10. Close the **Find Entries** page.

Task 2: Process the return of a purchase from return order to credit memo
-------------------------------------------------------------------------

### Scenario

While putting away stock, one of the delivered boxes of the 17” monitors turns
out to be damaged. Robert Townes will refund these items on return, which is
done on January 24th, 2023.

The purchase credit memo, with the same payment conditions as the invoice, and
with number 20-CN0747, is received by mail on February 3rd, 2023. The correct
amount of \$ 4,999.89 a box will be repaid to Contoso.

You will perform -

1.  Create a purchase return order

2.  Ship the items

3.  Create a posted purchase credit memo from the purchase return order

### Steps

1.  Create a purchase return order.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Purchase Return Orders`, and then choose the related link.

    2.  In the **Purchase Return Orders** list page, select **+ New**.

    3.  On the **General** FastTab, fill in the following fields:

        1.  In the **Vendor Name** field, enter **Robert Townes (V9002)**.

        2.  In the **Document Date** and **Order Date** fields, enter
            **1/24/2023**.

    4.  On the **Invoice Details** FastTab, in the **Payment Terms Code** field
        enter **30 DAYS**.

    5.  Select **Prepare**, and then select **Get Posted Document Lines to
        Reverse**…

    6.  In the opened page, fill in the following options:

        1.  Select the **Show Reversible Lines Only** checkbox

        2.  In the **Document Type Filter** field, enter the **Posted Invoices**
            option.

        3.  Select the line for item **CHW1003**.

        4.  Click **OK**.

    7.  On the **Lines** section on the purchase return order, select the line
        for **CHW1003** and then change the **Quantity** field to the value
        **1**.

    8.  Select **Release**.

2.  Ship the items.

    1.  On the **General** FastTab, click **Show more** and then fill in the
        following fields:

        1.  In the **Posting Date** field, enter **1/31/2023**.

        2.  In the **Vendor Cr. Memo No.** field, enter **20-CN0747**.

    2.  Select the dropdown next to **Posting**, and then select **Post**.

    3.  Select the **Ship** option and click **OK**.

3.  Create a posted purchase credit memo from the purchase return order.

    1.  On the **General** FastTab, fill in the following fields:

        1.  In the **Posting Date** field, enter **2/3/2023**.

        2.  In the **Vendor Cr. Memo No.** field, enter **20-CN0747**.

    2.  Select the dropdown next to **Posting**, and then select **Post**.

    3.  Select the **Invoice** option and click **OK**.

    4.  Click **No** to open the posted purchase credit memo.

Task 3: Process a purchase invoice for costs
--------------------------------------------

### Scenario

The accounting department at Contoso receives a cost invoice from vendor Robert
Townes, with an invoice date 3/6/2023 and invoice number OW-21-M2458. The
invoice needs to be paid within 15 days.

The invoice is for the monthly health and insurance cost of CAD 1,200.00, which
is processed per department.

The accounting manager has already set up a purchase recurring line for this
vendor (see Lab 4.2 exercise 4).

You need to process the invoice.

You will perform

1.  Process a purchase invoice using recurring purchase lines

### Steps

1.  Process a purchase invoice using recurring purchase lines

    1.  Select the Search icon in the top-right corner of the page,
        enter `Purchase Invoices`, and then choose the related link.

    2.  In the **Purchase Invoices** list page, select **+ New**.

    3.  On the **General** FastTab, fill in the following fields:

        1.  In the **Vendor Name** field, enter **Robert Townes (V9002)**.

        2.  In the **Posting Date** field, enter **3/6/2023**.

        3.  In the **Vendor Invoice No.** field, enter **OW-21-M2458**.

    4.  On the **Invoice Details** FastTab, in the **Payment Terms Code** field
        enter **15 DAYS**.

    5.  On the **Lines** section, the invoice lines for the health insurance per
        department are automatically filled in.

        1.  On the **Lines** field, add a new line and enter **Item** in the
            **Type** field.

        2.  Enter the item **CHW1002** in the **No.** field.

        3.  Enter **4** in the **Quantity** field.

    6.  Select **Post**.

    7.  Click **Yes** to post.

    8.  Click **No** to open the posted invoice.
