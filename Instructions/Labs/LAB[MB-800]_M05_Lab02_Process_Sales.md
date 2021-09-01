---
lab:
    title: 'Lab: Process Sales'
    module: 'Module 5: Operations'
---

## Exercise 1: Process a sales from quote to invoice

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

On January 16th, 2021, a quote is created by Debra L. Core for the following
items:

-   1 box of the 15” flat panels, at the current price of \$ 4,800.00 a box with
    a 6% discount for all medium-sized companies.

-   3 pieces of the 17” monitor, at the current price of \$ 700.00 a piece with
    a 6% discount for all medium-sized companies.

The potential customer now has 10 days to either accept or turn down the
proposal.

On January 22nd, 2021 Francematic accepts the sales quote and the quote is
turned into an order.

The items are shipped to the customer on 2 different dates:

-   On January 25th, 2021, the 15” flat panels are delivered.

-   On January 27th, 2021, the 17” monitors are delivered.

On January 28th, 2021, the sales invoice is created and send to the customer.

### Tasks

1.  Create a contact.

2.  Create a sales quote for a contact.

3.  Process the quote into an order.

4.  Partially ship items from the order.

5.  Create a posted sales invoice from the sales order.

### Task 1: Create a contact.

2.  At the top of the page, click the search icon in the black bar on the right. Then type **Contacts** and click the **Contacts** link.

3.  In the **Contacts** list page, select **New**.

4.  On the **General** FastTab, fill in the following fields:

     1.  In the **Name** field, enter ‘Francematic’.

     2.  In the **Type** field, leave the default value **Company**.

5.  On the **Communication** FastTab, fill in the following fields:

     1.  In the **Address** field, enter ‘19 Boulevard Commanderie’.

     2.  In the **Country/Region Code** field, enter FR.

     3.  In the **ZIP Code** field, enter FR-78370.

     4.  The **City** field is automatically filled in with the value PLAISIR.

6.  On the **Foreign Trade** FastTab, leave the **Currency Code** field blank.

### Task 2: Create a sales quote for a contact.

1.  On the **Contacts** list page, select the new contact Francematic.

9.  Select **Process** and then select **Create Sales Quote**.

10. Click **Yes** for selecting a customer template.

11. In the opened **Contact Conversion Templates** page, select **New**.

12. In the customer template card, fill in the following fields:

      1.  In the **Code** field, enter CUST EU.

      2.  In the **Description** field, enter ‘Customer EU’.

      3.  In the **Contact Type** field, leave the default value ‘Company’.

      4.  Leave the **Currency Code** field blank.

      5.  In the **Gen. Bus. Posting Group** field, enter EU.

      6.  The **VAT Bus. Posting Group** field is automatically filled in with the value EU.

      7.  In the **Customer Posting Group** field, enter FOREIGN.

      8.  In the **Customer Price Group** field, enter EU.

      9.  In the **Customer Disc. Group** field, enter MEDIUM.

      10. In the **Payment Terms Code** field, enter ‘0 DAYS’.

      11. Select **Dimensions**, and fill in the following fields:

      12. In the **Dimension Code** field, enter CUSTOMERGROUP

      13. In the **Dimension Value Code** field, enter MEDIUM

      14. Close the customer template card.

13. Click **OK** to apply the new customer template card and create a new sales quote.

14. A new sales quote is created.

15. In the **General** FastTab, fill in the following fields (you may need to click **Show more**:

     1.  In the **Order Date** and **Document Date** field, enter 1/15/2021.

     2.  In the **Quote Valid To Date** field, enter 1/25/2021.

     3.  In the **Salesperson Code** field, enter JO.

16. On the **Lines** section, enter a new line by filling in the following fields:

     1.  In the **Type** field, enter **Item**.

     2.  In the **No.** field, enter CHW1002 for the 15” flat panels.

     3.  In the **Location Code** field, enter EUROP.

     4.  In the **Unit of Measure Code** field, enter BOX.

     5.  In the **Quantity** field, enter 1.

     6.  In the **Unit Price Excl. Tax** field, the value 4,800.00 is automatically filled in.

     7.  In the **Line Discount %** field, the value ‘6’ is automatically filled in.

17. On the **Lines** section, enter a new line by filling in the following fields:

     1.  In the **Type** field, enter **Item**.

     2.  In the **No.** field, enter CHW1003 for the 17” flat panels.

     3.  In the **Location Code** field, enter EUROP.

     4.  In the **Unit of Measure Code** field, leave the default value PCS.

     5.  In the **Quantity** field, enter 3.

     6.  In the **Unit Price Excl. Tax** field, the value 700.00 is automatically filled in.

     7.  In the **Line Discount %** field, the value ‘6’ is automatically filled in.

### Task 3: Process the quote into an order.

1. On the **Sales Quote** card page, change the **Order Date** field to
    1/22/2021. Click **OK**.

20. Select **Process** and then select **Make Order**.

21. Click **Yes**.

22. Click **Yes** to create a customer card for contact Francematic.

23. Click **OK**.

24. Click **Yes** to open the sales order.

### Task 4: Partially ship items from the order.

1. On the **Sales Order** card page, on the **General** FastTab, in the
    **Posting Date** field, enter 1/25/2021.

27. On the **Lines** FastTab, select the line for the 17” monitors.

28. In the **Qty. to Ship** field, remove the value, and leave the field
    blank.

29. Select **Posting** and then select **Post**.

30. Select the **Ship** option and click **OK**.

31. On the **General** FastTab, in the **Posting Date** field, enter
    1/27/2021.

32. Select **Posting** and then select **Post**.

33. Select the **Ship** option and click **OK**.

### Task 5: Create a posted sales invoice from the sales order.

1. On the **Sales Order** card page, on the **General** FastTab, in the
    **Posting Date** field, enter 1/28/2021.

36. Select **Posting** and then select **Post**.

37. Select the **Invoice** option and click **OK**.

38. Review the posted sales invoice.

39. In the **Posted Sales Invoices** list page, select the invoice for
    customer Francematic.

40. Select **More options**, select **Actions** and then select **Find entries**.

41. Select the line for G/L entries sand select **Show Related Entries**.

    ![General ledger entries](media/lab5_2_general_ledger_entries.png)

42. Close the **G/L entries** page.

43. Close the **Find Entries** page.

## Exercise 2: Process a sales invoice for multiple orders

### Scenario

During the month January the web shop sales has been picking up and a lot of
items were shipped to private customers.

First record a couple of these sales orders and shipments for the generic EU
customer as follows:

| Order & Delivery Date | Reference       | Shipment Address | Qty.  | Item    |
|-----------------------|-----------------|------------------|-------|---------|
| 1/26/2021             | Private sale DK | PICK-UP-DK       | 2 PCS | CHW1002 |
| 1/27/2021             | Private sale BE | PICK-UP-BE       | 1 BOX | CHW1002 |
| 1/28/2021             | Private sale FR | PICK-UP-FR       | 5 PCS | CHW1003 |

At the end of the month, 1 combined invoice is created for all private sales.
You must now create this sales invoice for the generic EU customers, containing
all shipments of January, including the 5% web shop discount for the month
January.

### Tasks

1.  Create several sales orders and shipments.

2.  Use the Combine Shipments function to create sales invoices.

### Task 1: Create several sales orders and shipments.

2.  At the top of the page, click the search icon in the black bar on the right. Then type **Customers** and click the **Customers** link.

3.  On the **Customers** list page, select the generic EU customer.

4.  Select **New Document** and then select **Sales Order**.

5.  On the opened **Sales Order** card page, on the **General** FastTab, fill in the following fields:

     1.  In the **Order Date** field, enter 1/26/2021.

     2.  In the **Posting Date** field, enter 1/26/2021.

     3.  In the **Your Reference** field, enter ‘Private sale DK’.

6.  On the **Shipping and Billing** FastTab, fill in the following fields:

     1.  In the **Ship-to** field, select the **Alternate Shipping Address** option.

     2.  On the opened **Ship-to Address** List page, select PICK-UP-DK and click **OK**.

     3.  Select the **Combine Shipments** checkbox.

7.  On the **Lines** section, enter a new line by filling in the following fields:

     1.  In the **Type** field, enter **Item**.

     2.  In the **No.** field, enter CHW1002.

     3.  In the **Location Code** field, the value EUROP is automatically filled in.

     4.  In the **Unit of Measure Code** field , the value PCS is automatically filled in.

     5.  In the **Quantity** field, enter ‘2’.

8.  Select **Posting** and then select **Post**.

9.  Select the **Ship** option and click **OK**.

10. Click **OK** for the sales order to be placed in a job queue.

11. Close the **Sales Order** page.

12. On the **Customers** list page, select the generic EU customer.

13. Select **New Document** and then select **Sales Order**.

14. On the opened **Sales Order** card page, on the **General** FastTab, fill in the following fields:

     1.  In the **Order Date** field, enter 1/28/2021.

     2.  In the **Posting Date** field, enter 1/28/2021.

     3.  In the **Your Reference** field, enter ‘Private sale BE’.

15. On the **Shipping and Billing** FastTab, fill in the following fields:

     1.  In the **Ship-to** field, select the **Alternate Shipping Address** option.

     2.  On the opened **Ship-to Address** List page, select PICK-UP-BE and click **OK**.

     3.  Select the **Combine Shipments** checkbox.

16. On the **Lines** section, enter a new line by filling in the following fields:

     1.  In the **Type** field, enter **Item**.

     2.  In the **No.** field, enter CHW1002.

     3.  In the **Location Code** field, the value EUROP is automatically filled in.

     4.  In the **Unit of Measure Code** field , enter BOX.

     5.  In the **Quantity** field, enter ‘1’.

17. Select **Posting** and then select **Post**.

18. Select the **Ship** option and click **OK**.

19. Click **OK** for the sales order to be placed in a job queue.

20. Close the **Sales Order** page.

21. On the **Customers** list page, select the generic EU customer.

22. Select **New Document** and then select **Sales Order**.

23. On the opened **Sales Order** card page, on the **General** FastTab, fill in the following fields:

     1.  In the **Order Date** field, enter 1/29/2021.

     2.  In the **Posting Date** field, enter 1/29/2021.

     3.  In the **Your Reference** field, enter ‘Private sale FR’.

24. On the **Shipping and Billing** FastTab, fill in the following fields:

      1.  In the **Ship-to** field, select the **Alternate Shipping Address** option.

      2.  On the opened **Ship-to Address** List page, select PICK-UP-FR and click **OK**.

      3.  Select the **Combine Shipments** checkbox.

25. On the **Lines** section, enter a new line by filling in the following fields:

     1.  In the **Type** field, enter **Item**.

     2.  In the **No.** field, enter CHW1003.

     3.  In the **Location Code** field, the value EUROP is automatically filled in.

     4.  In the **Unit of Measure Code** field , the value PCS is automatically filled in.

     5.  In the **Quantity** field, enter ‘5’.

26. Select **Posting** and then select **Post**.

27. Select the **Ship** option and click **OK**.

28. Click **OK** for the sales order to be placed in a job queue.

29. Close the **Sales Order** page.

### Task 2: Use the Combine Shipments function to create sales invoices.

31. Open the **Combine Shipments** task.

32. In the **Posting Date** and **Document Date** field, enter 1/31/2021.

33. Select the **Calc. Inv. Discount** checkbox.

34. Select the **Post Invoices** checkbox.

35. In the **Sell-to Customer No.** filter, enter CWEB0001.

36. Click **OK**.

37. Click **OK**.

## Exercise 3: Correct a posted sales invoice

### Scenario

The new customer Francematic complaint that only 2 of the 3 17” monitors were
delivered.

You need to make a sales credit memo on January 31st, 2021, to refund 1 piece of
this item.

### Tasks

1.  Correct a posted sales invoice

### Task 1: Correct a posted sales invoice

2.  At the top of the page, click the search icon in the black bar on the right. Then type **Posted Sales Invoices** and click the **Posted Sales Invoices** link.

3.  On the **Posted Sales Invoices** list page, select the invoice for customer Francematic.

4.  Select **Correct** and then select **Create Corrective Credit Memo**.

5.  On the opened sales credit memo, on the **General** FastTab, in the **Posting Date** field, enter 1/31/20201.

6.  On the **Lines** section, delete the line for the 15” flat panels.

7.  On the **Lines** section, select the line for the 17” monitors.

8.  Change the **Quantity** field from ‘3’ to ‘1’.

9.  Select **Posting** and then select **Post**.

10. Click **Yes**.

11. Click **OK**.
