
---
lab:
    title: 'Lab: Process Purchases'
    module: 'Module 5: Operations'
---

## Exercise 1: Process a purchase from order to invoice and review the posted documents

### Scenario

As the purchasing agent you are replenishing the stock for the European
warehouse. The computer monitors are currently low on stock and a purchase order
with their main vendor Cronus Cardoxy Sales is placed on January 14th, 2021. It
was agreed to always invoice in USD instead of their currency (DKK) and a
purchase request is sent to the correct order address for the following items to
be delivered on January 19th, 2021:

-   100 pieces of the 15” flat panel at \$ 4,999.89 a box, containing 10 pieces.

-   50 pieces of the 17” monitor at \$ 5,348.56 a box, containing 10 pieces

The purchase request is confirmed by the vendor on January 15th, 2021 with order
confirmation OC15-479. They mention a delivery delay of a couple of days,
expecting to be able to deliver the entire order on January 22nd, 2021.

Eventually the goods are delivered with delivery note DN01-47 on January 23rd,
2021 as follows:

-   11 boxes of the 15” flat panel – this is 1 box more than ordered

-   4 boxes of the 17” monitor – this is 1 box less than ordered

The purchase invoice with number 20-0747 is received by mail on January 26th,
2021 where a 5% discount is granted on the 15” monitors as a compensation for
the delivery delay. The invoice needs to be paid within 30 days.

### Tasks

1.  Change the currency code on the vendor.

2.  Create a purchase order.

3.  Receive items on the purchase order.

4.  Create a posted purchase invoice from the purchase order.

5.  Review the posted purchase receipt and invoice.

### Task 1: Change the currency code on the vendor.

1.  On the **Vendors** list page, select vendor Cronus Cardoxy Sales

2.  Select **Manage** and then select **Edit**.

3.  On the opened vendor card, go to the **Invoicing** FastTab, and in the
        **Currency Code** field remove the value DKK and leave the field blank.

### Task 2: Create a purchase order.

1.  On the vendor card, select **New Document** and then select **Purchase
        Order**.

2.  On the **General** FastTab, fill in the following fields:

    1.  In the **Document Date** and **Order Date** fields, enter 1/14/2021.

    2.  In the **Alternate Vendor Address Code** field, enter COMP&MON.

    3.  In the **Vendor Order No.** field, enter OC15-479.

3.  On the **Invoice Details** FastTab, fill in the following fields:

    1.  In the **Requested Receipt Date** field, enter 1/19/2021.

    2.  In the **Promised Receipt Date** field, enter 1/22/2021.

4.  On the **Lines** section, enter a new line by filling in the following
        field:

    1.  In the **Type** field, enter **Item**.

    2.  In the **No.** field, enter CHW1002 for the 15” flat panels.

    3.  In the **Location Code** field, the value EUROP is automatically
            filled in.

    4.  In the **Unit of Measure Code** field, the value BOX is
            automatically filled in.

    5.  In the **Quantity** field, enter ‘10’.

    6.  In the **Direct Unit Cost Excl. Tax** field, enter ‘4,999.89’.

5.  On the **Lines** section, enter a new line by filling in the following
        field:

    1.  In the **Type** field, enter **Item**.

    2.  In the **No.** field, enter CHW1003 for the 17” flat panels.

    3.  In the **Location Code** field, the value EUROP is automatically
            filled in.

    4.  In the **Unit of Measure Code** field, the value BOX is
            automatically filled in.

    5.  In the **Quantity** field, enter ‘5’.

    6.  In the **Direct Unit Cost Excl. Tax** field, enter ‘5,348.56’.

    6.  Select **Release**.

### Task 3: Receive items on the purchase order.

1.  On the **General** FastTab, fill in the following fields:

    1.  In the **Posting Date** field, enter 1/23/2021.

    2.  In the **Vendor Shipment No.** field, enter ‘DN01-47’.

2.  On the **Lines** section, select the line for item CHW1002, and fill in
        the following fields:

    1.  In the **Over-Receipt Code** field, enter OVERRCPT10.

    2.  In the **Qty. to Receive** field, enter ‘11’.

3.  On the **Lines** section, select the line for item CHW1003, and fill in
        the following fields:

    1.  In the **Qty. to Receive** field, enter ‘4’.

    4.  Select **Posting**, and then select **Post**.

    5.  Select the **Receive** option, and click **OK**.

### Task 4: Create a posted purchase invoice from the purchase order.

1.  Select **Release**, and then select **Reopen**.

2.  On the **General** FastTab, fill in the following fields:

    1.  In the **Posting Date** field, enter 1/24/2021.

    2.  In the **Vendor Invoice No.** field, enter ‘20-0747’.

3.  On the **Invoice Details** FastTab, in the **Payment Terms Code** field,
        enter ’30 DAYS’.

4.  On the **Lines** section, select the line for item CHW1002, and fill in
        the following fields:

    1.  In the **Line Discount%** field, enter ‘5’.

5.  Select **Posting**, and then select **Post**.

6.  Select the **Invoice** option, and click **OK**.

### Task 5: Review the posted purchase receipt and invoice.

1.  Select **Related**, then select **Documents**, and then select
        **Receipts**.

2.  In the page, select the posted purchase receipt.

3.  Select **Actions**, and then select **Find Entries**.

4.  Select the line for **Item Ledger Entry** and select **Show Related
        Entries**.

![Item ledger entries](media/lab5_1_item_ledger_entries.png)

6.  Close the **General Ledger Entries** page.

    1.  Close the **Find Entries** page.

    2.  Select **Related**, then select **Documents**, and then select
       **Invoices**.

    3.  In the page, select the posted purchase invoice.

    4.  Select **Reports**, and then select **Find Entries**.

    5.  Select the line for G/L entries and select **Show Related Entries**.

![General ledger entries](media/lab5_1_general_ledger_entries.png)

6.  Close the **General Ledger Entries** page.

7.  Close the **Find Entries** page.

## Exercise 2: Process the return of a purchase from return order to credit memo

### Scenario

While putting away stock, one of the delivered boxes of the 17” monitors turns
out to be damaged. Cronus Cardoxy Sales will refund these items on return, which
is done on January 24th, 2021.

The purchase credit memo, with the same payment conditions as the invoice, and
with number 20-CN0747, is received by mail on January 31st, 2021. The correct
amount of \$ 4,999.89 a box will be repaid to Contoso.

### Tasks

1.  Create a purchase return order

2.  Ship the items

3.  Create a posted purchase credit memo from the purchase return order

### Task 1: Create a purchase return order.

1.  In the **Purchase Return Orders** list page, select **New**.

2.  On the **General** FastTab, fill in the following fields:

    1.  In the **Vendor Name** field, enter ‘V9002’.

    2.  In the **Document Date** and **Order Date** fields, enter 1/24/2021.

3.  On the **Invoice Details** FastTab, in the **Payment Terms Code** field
        enter ‘30 DAYS’.

4.  Select **Process**, and then select **Get Posted Document Lines to
        Reverse**…

5.  In the opened page, fill in the following options:

    1.  Select the **Show Reversible Lines Only** checkbox

    2.  In the **Document Type Filter** field, enter the **Posted Invoices**
            option.

    3.  Select the line for item CHW1003.

    4.  Click **OK**.

6.  On the **Lines** section on the purchase return order, change the
        **Quantity** field to the value ‘1’.

7.  Select **Release**.

### Task 2: Ship the items.

1.  On the **General** FastTab, fill in the following fields:

    1.  In the **Posting Date** field, enter 1/31/2021.

    2.  In the **Vendor Cr. Memo No.** field, enter ‘20-CN0747’.

2.  Select **Posting**, and then select **Post**.

3.  Select the **Ship** option and click **OK**.

### Task 3: Create a posted purchase credit memo from the purchase return order.

1.  On the **General** FastTab, fill in the following fields:

    1.  In the **Posting Date** field, enter 1/31/2021.

    2.  In the **Vendor Cr. Memo No.** field, enter ‘20-CN0747’.

2.  Select **Posting**, and then select **Post**.

3.  Select the **Invoice** option and click **OK**.

4.  Click **No** to opening the posted purchase credit memo.

## Exercise 3: Process a purchase invoice for costs

### Scenario

The accounting department at Contoso, receives a cost invoice from vendor
OakvilleWorld, with an invoice date 1/31/2021 and invoice number OW-21-M2458.
The invoice needs to be paid within 15 days.

The invoice is for the monthly health and insurance cost of CAD 1,200.00, which
is processed per department.

The accounting manager has already set up a purchase recurring line for this
vendor (see Lab 4.2 exercise 4).

You need to process the invoice.

### Tasks

1.  Process a purchase invoice using recurring purchase lines

### Task 1: Process a purchase invoice using recurring purchase lines

1.  In the **Purchase Invoices** list page, select **New**.

2.  On the **General** FastTab, fill in the following fields:

    1.  In the **Vendor Name** field, enter ‘V9002’.

    2.  In the **Posting Date** field, enter 1/31/2021.

    3.  In the **Vendor Invoice No.** field, enter OW-21-M2458.

3.  On the **Invoice Details** FastTab, in the **Payment Terms Code** field
       enter ‘15 DAYS’.

4.  On the **Lines** section, the invoice lines for the health insurance per
        department are automatically filled in.

5.  Select **Posting** and then select **Post**.

6.  Click **Yes** to post.

7.  Click **No** to opening the posted invoice.
