---
lab:
  title: 'Lab 06: Configure item costing'
  module: 'Set up general ledger configuration options in Dynamics 365 Business Central'
  duration: 90 minutes
  level: 300
  islab: true
---

## Exercise: Configure item costing

## Task 1. Apply the Average costing method.

## Scenario
The company is a retail business that has historically valued its inventory using the Average Cost method, with the average calculated over the month. As the accountant, your task is to record several retail purchase and sales transactions for December 2025, all posted to the EUROPE location.

Purchase documents:


| Document Date | Vendor Name | Vendor Document number | Item | Quantity, Pieces | Price $ |
| --- | --- | --- | --- | --- | --- |
| 12/1/2025 | Wide World Importers | WW25/367 | Computer III 533 MHz | 2 | 800 |
| 12/10/2025 | Wide World Importers | WW25/368 | Computer III 533 MHz | 1 | 1000 |


Sales documents:


| Document Date | Customer Name | Customer Order No. | Item | Quantity, Pieces | Price $ |
| --- | --- | --- | --- | --- | --- |
| 12/16/2025 | Trey Research | 25-0111 | Computer III 533 MHz | 1 | 1800 |
| 12/25/2025 | Trey Research | 25-0201 | Computer III 533 MHz | 1 | 1800 |
| 12/26/2026 | Trey Research | 25-0202 | Computer III 533 MHz | 1 | 1800 |

After registering the documents, you need to check that the item has an average cost and check its transactions.

You will perform:

- Set up the Average costing method for inventory.

- Configure costing method for new item card.

- Register item purchases.

- Register item sales.

- Analise cost and posted entries related to items.

### Steps
1. Set up the Average costing method for inventory.
Select the Search icon in the top-right corner of the page, enter Inventory Setup, and then choose the related link.
In the Inventory Setup page, go to the General FastTab, select More.

2. In the Default Costing Method field, select Average option.

3. In the Average Cost period field, select Month option.

4. Configure costing method for new item card.

    a. Select the Search for page icon in the top-right corner of the page, enter Items, and then choose the related link.

    b. On the Items page, select item Computer III 533 MHz CHW1000.

    c. In the Item card page, go to Cost&Posting FastTab.

	d. In the Costing method field, select Average option.

    e. Close the item card.

5. Register item purchases.

    a. Select the Search for page icon in the top-right corner of the page, enter Purchase Orders , and then choose the related link.

    b. Select +New and select in the Vendor No. field vendor 40000 Wide World Importers.

    c. On the General FastTab, select Show more and then fill in the following fields: 

	1. In the Document Date, Posting Date fields, enter 12/1/2025. 
	2. In the Vendor Address field, enter 123 Main Street.
	3. In the Vendor Invoice No. field, enter WW25/367.

6. On the Lines section, enter a new line by filling in the following field: 

	1. In the Type field, enter Item. 
	2. In the No. field, enter CHW1000 for the  Computer III 533 MHz. 
	3. In the Location Code field, select the value EUROP. 
	4. In the Unit of Measure Code field, the value PCS is automatically filled in. 
	5. In the Quantity field, enter 2. 
	6. In the Direct Unit Cost Excl. Tax/VAT field, enter 800. 
	7. In the Posting field, select Post.
	8. Select Receive and Invoice, select OK. 
	9. Select No to open the posted purchase invoice.
7.  Repeat step actions to enter and post the purchase document WW25/368 on 12/10/2025.

8. Register item sales.
   1. Select the Search icon in the top-right corner of the page, enter Sales Orders and then choose the related link.
   2. On the Sales Orders list page, select +New.
   3. On the opened Sales Order card page, on the General FastTab, select Show more and then fill in the following fields:
      1. In the Customer No. field, enter 20000 Trey Research
      2. In the Document Date, Posting Date fields, enter 12/16/2025.
      3. In the External Document No. field, enter 25-0111.
   4. On the Lines section, enter a new line by filling in the following fields:
      1. In the Type field, enter Item.
      2. In the No. field, enter CHW1000 Computer III 533 MHz.
      3. In the Location Code field, select the value EUROP.
      4. In the Unit of Measure Code field, the value PCS is automatically filled in.
      5. In the Quantity field, enter 1.
      6. In the Unit Price Excl.Tax/VAT enter 1800.
      7. In the Tax Group Code field, enter NONTAXABLE.

9. Select Home and then select Post.

10. Select the Ship and Invoice option and select OK.
11. Select No to open the posted sales invoice.
12. Repeat step actions to enter and post the sales documents 25-0201 on 12/25/2025, 25-0202 on 12/26/2026.

13. Analyze item cost on item card.
    1.  Select the Search icon in the top-right corner of the page, enter Items and then choose the related link.
    2.  On the opened Items list page, select Item No. CHW1000, select Manage, View.
    3.  In the Item card page, go to Cost&Posting FastTab.
    4.  Check the Unit cost field has value 866.66 and the Last Direct Cost field has value of the last purchase 1000.

14. Analyze Item Ledger Entries.
    1.  Select on the menu Related, History, Entries, Item Ledger Entries.
    2.  Sort by the Posting date field.
    3.  Ensure that all sales entries show the same average Cost Amount (Actual). The average cost should equal: Sum of Purchase Cost Amount (Actual) ÷ Sum of Purchase Quantity

NOTE: Amount may differ by 0.01 because of rounding.



| Posting Date | Entry Type | Document Type | Item No. | Quantity | Sales Amount (Actual) | Cost Amount (Actual) |
| --- | --- | --- | --- | --- | --- | --- |
| 12/01/2025 | Purchase | Purchase Receipt | CHW1000 | 2 | 0.00 | 1,600.00 |
| 12/10/2025 | Purchase | Purchase Receipt | CHW1000 | 1 | 0.00 | 1,000.00 |
| 12/16/2025 | Sale | Sales Shipment | CHW1000 | -1 | 1,800.00 | -866.67 |
| 12/25/2025 | Sale | Sales Shipment | CHW1000 | -1 | 1,800.00 | -866.67 |
| 12/26/2025 | Sale | Sales Shipment | CHW1000 | -1 | 1,800.00 | -866.66 |

15. Related Value entries and G/L entries.
16. In the Item ledger entries list, select the last sales entries from 12/16/25.
17. Select on the menu of Entry, Value Entries.
18. Verify that the Value entry shows:
    1.  Sales Amount (Actual): 1800
    2.  Cost Amount (Actual): 866.67 
    3.  This cost amount should match the average cost for the period for this item.
19. Select Find Entries, G/L Entry to view the related general ledger postings linked to the value entry.
20. Close General Ledger entries page.
21. Close Find entries page.
22. Close Value Entries page.

23. Applied item entries.
    1.  In the Item ledger entries list, select in the menu Application Worksheet.
    2.  On the Application Worksheet page, select the Item filter field CHW1000.
    3.  Select the line with sales entry from 12/16/25, the first sales for this item.
    4.  Select Applied Entries.
    5.  Make sure that you see the purchase entry from 12/1/25. This is the first purchase entry for this item.
    6.  Close View Applied Entries page.
24. Close Application Worksheet page.


## Task 2: Change to FIFO costing method.

## Scenario
The company is entering a new fiscal year and management has decided to move from the Average Cost method to the FIFO (First
In, First
Out) costing method. As the accountant, your responsibility is to ensure the transition is handled correctly and that new transactions follow FIFO rules.

You begin by reviewing the inventory quantities at the EUROPE location to confirm what stock remains from the previous year. Once verified, you proceed to repost inventory using the FIFO costing method, ensuring that all new cost layers created in the new fiscal year follow FIFO valuation. After the costing method is updated, you record several retail purchase and sales transactions for January 2026, all posted to the EUROPE location.


| Document Date | Vendor Name | Vendor Document number | Item | Quantity, Pieces | Price $ |
| --- | --- | --- | --- | --- | --- |
| 1/1/2026 | Wide World Importers | WW26/001 | Computer III 533 MHz | 2 | 800 |
| 1/10/2026 | Wide World Importers | WW26/002 | Computer III 533 MHz | 1 | 1000 |

Sales documents:


| Document Date | Customer Name | Customer Order No. | Item | Quantity, Pieces | Price $ |
| --- | --- | --- | --- | --- | --- |
| 1/16/2026 | Trey Research | 26-0111 | Computer III 533 MHz | 1 | 1800 |
| 1/25/2026 | Trey Research | 26-0201 | Computer III 533 MHz | 1 | 1800 |
| 1/26/2026 | Trey Research | 26-0202 | Computer III 533 MHz | 1 | 1800 |

After registering the documents, you need to check that the item has an average cost and check its transactions.


You will perform:

- Set up the FIFO costing method for inventory.

- Copy an item and assign FiFO costing method.

- Register item purchases.

- Register item sales.

- Analise cost and posted entries related to items.

### Steps
1. Set up the FIFO costing method for inventory.
   1. Select the Search icon in the top-right corner of the page, enter Inventory Setup, and then choose the related link.
   2. In the Inventory Setup page, go to the General FastTab, select More.
   3. In the Default Costing Method field, select FIFO option.
2. Copy an item and assign FiFO costing method.
   1. Select the Search for page icon in the top-right corner of the page, enter Items, and then choose the related link.
   2. On the Items page, select item Computer III 533 MHz CHW1000, Edit.
   3. Select the menu for Home, Copy Item.
   4. On the Copy Item page
   5. In the Source Item No. field, the value  CHW1000 is automatically filled in.
   6. In the Target No. Series field, select the value COMPHW.
   7. In the Number of copies field, leave value 1.
   8.  Select the Copy all information and Show Created items fields.
   9.  Select OK.
3.  On the item CHW1006 Computer III 533 MHz card page, on the Cost&Posting  FastTab
    1.  In the Costing method field, select the value FIFO.
    2.  In the Unit Cost and Last Direct Cost select the value 0.
    3.  Close the item card.
4.  Register item purchases.
    1.  Select the Search for page icon in the top-right corner of the page, enter Purchase Orders, and then choose the related link.
    2.  Select +New and select in the Vendor No. field vendor 40000 Wide World Importers.
    3.  On the General FastTab, select Show more and then fill in the following fields: 
        1.  In the Document Date, Posting Date fields, enter 1/1/2026. 
        2.  In the Vendor Invoice No. field, enter WW26/001.
    4.  On the Lines section, enter a new line by filling in the following fields: 
        1.  In the Type field, enter Item. 
        2.  In the No. field, enter CHW1006 for the  Computer III 533 MHz. 
        3.  In the Location Code field, select the value EUROP. 
        4.  In the Unit of Measure Code field, the value PCS is automatically filled in. 
        5.  In the Quantity field, enter 2. 
        6.  In the Direct Unit Cost Excl. Tax/VAT field, enter 800. 
    5.  Select the dropdown of Posting, and then select Post. 
    6.  Select Receive and Invoice, select OK. 
    7.  Select No to open the posted purchase invoice.
    8.  Repeat step actions to enter and post the purchase document WW26/002 on 1/10/2026.

5. Register item sales.
   1. Select the Search icon in the top-right corner of the page, enter Sales Orders and then choose the related link.
   2. On the Sales Orders list page, select +New.
   3. On the opened Sales Order card page, on the General FastTab, select Show more and then fill in the following fields:
       4. In the Customer No. field, enter 20000 Trey Research
       5. In the Document Date, Posting Date fields, enter 1/16/2026.
       6. In the External Document No. field, enter 26-0111.
    4. On the Lines section, enter a new line by filling in the following fields:
       1.  In the Type field, enter Item.
       2.  In the No. field, enter CHW1006 Computer III 533 MHz.
       3.  In the Location Code field, select the value EUROP.
       4.  In the Unit of Measure Code field, the value PCS is automatically filled in.
       5.  In the Quantity field, enter 1.
       6.  In the Unit Price Excl.Tax/VAT enter 1800.
       7.  In the Tax Group Code field, enter NONTAXABLE.
   4.  Select Home and then select Post.
   5.  Select the Ship and Invoice option and select OK.
   6.  Select No to open the posted sales invoice.
   7.  Repeat step actions to enter and post the sales document 26-0201 on 1/25/2026, 26-0202 on 1/26/2026
6.  Analyze posted entries related to items.
    1.  Analyze item cost on item card.
        1.  Select the Search icon in the top-right corner of the page, enter Items and then choose the related link.
        2.  On the opened Items list page, select Item No. CHW1003, select Manage, View.
        3.  In the Item card page, go to Cost&Posting FastTab.
        4.  Check the Unit cost field has value 1000 and the Last Direct Cost field has value of the last purchase 1000.
7.  Analyze Item Ledger Entries.
    1.  Select on the menu Related, History, Entries, Item Ledger Entries.
    2.  Sort by the Posting date field.
    3.  Ensure that the sales entries show different Cost Amount (Actual) values.

| Posting Date | Entry Type | Document Type | Item No. | Quantity | Sales Amount (Actual) | Cost Amount (Actual) |
| --- | --- | --- | --- | --- | --- | --- |
| 01/01/2026 | Purchase | Purchase Receipt | CHW1006 | 2 | 0.00 | 1,600.00 |
| 10/01/2026 | Purchase | Purchase Receipt | CHW1006 | 1 | 0.00 | 1,000.00 |
| 16/01/2026 | Sale | Sales Shipment | CHW1006 | -1 | 1,800.00 | -800.00 |
| 25/01/2026 | Sale | Sales Shipment | CHW1006 | -1 | 1,800.00 | -800.00 |
| 26/01/2026 | Sale | Sales Shipment | CHW1006 | -1 | 1,800.00 | -1,000.00 |

8.  Related Value entries and G/L entries.
    1.  In the Item ledger entries list, select the last sales entry dated 1/16/26.
    2.  From the menu, select Entry, Value Entries.
    3.  Verify that the Value entry shows:
        1.  Sales Amount (Actual) 1800
        2.  Cost Amount (Actual) 800, this amount should match the unit cost from the first purchase.
    4.  Select Find Entries, G/L Entry to view the related general ledger postings.
9.  Close General Ledger entries page.
10. Close Find entries page.
11. Close Value Entries page.

12. Applied item entries.
    1.  In the Item ledger entries list, select the sales entry dated 1/16/26.
    2.  On the menu, select Entry, Applied entries.
    3.  Confirm that the applied entries include the purchase entry dated 1/1/26, which represents the first purchase for this item.
Close Applied Item entries page.