---
lab:
  title: 'Lab 23: Perform finance operations'
  module: 'Create and process journal entries in Dynamics 365 Business Central'
  duration: 60 minutes
  level: 300
  islab: true
---


## Exercise 23: Perform finance operations.


## Task 1: Create and post opening balances.

## Scenario
You are a functional consultant and are working on opening balances for the Contoso company.

The accounting manager at Contoso has provided you with a summary of opening balances by general ledger account as of 12/31/2025.



| Account no. | Account name | Amount, $ |
| --- | --- | --- |
| 10400 | Opening Customer Entries | 14375.40 |
| 20100 | Opening Vendor Ledger | -34871.27 |
| 10100 | Bank Account – Operating | 20495.87 |

One week later, an accountant provided detailed balances:

Customer detailed balances:


| Account no. | Account name | Document Date | Document No. | Amount, $ |
| --- | --- | --- | --- | --- |
| 10000 | Adatum Corporation | 10/01/25 | INV251001 | 1000 |
| 10000 | Adatum Corporation | 10/20/25 | INV251002 | 3600 |


| Account no. | Account name | Document Date | Document No. | Amount, $ |
| --- | --- | --- | --- | --- |
| 10000 | Fabrikam, Inc. | 10/10/25 | 25-034 | -5000 |
| 10000 | Fabrikam, Inc. | 10/20/25 | 25-356 | -3600 |


| Account no. | Account name | Document Date | Document No. | Amount, $ |
| --- | --- | --- | --- | --- |
| CHECKING | CHECKINGS bank account | 12/31/25 | OPENBAL2 | 20495,87 |

You will perform:

- Record open balances by general ledger accounts.

- Reallocate open balances to specific accounts.


- Step 1. Record open balances by general ledger accounts.


Select the Search icon in the top-right corner of the page, enter General Journals and then choose the related link.

In the General Journal Template page select OPENING.

- On the General Journals list page, select the OPENING journal.

- Open the assist edit button to the right of the Batch Name field.

- Select the BALANCE journal batch.

- Select OK.

- Select the first line and fill in the following details. 
Enter 12/31/25 the Posting Date field

- Enter OPENBAL2 in the Document No. field

- Enter 10400 in the Account No. field

- Enter 14375.40 in the Amount field


- Select the new line and fill in the following details. 
Enter 12/31/25 the Posting Date field

- Enter OPENBAL2 in the Document No. field  
Enter 20100 in the Account No. field

- Enter  -34871.27 in the Amount field


- Select the new line and fill in the following details. 
Enter 12/31/25 the Posting Date field

- Enter OPENBAL2 in the Document No. field  
Enter 10100 in the Account No. field 
Enter  20495.87 in the Amount field


Select Post -> Preview Posting

Check for any errors and correct them

- Close the window

- Select Post

- Select Yes

- Select OK

- Close the General Journals Page.


- Step 2. Reallocate open balances to specific accounts.

Enter General Journals in the search and select the related link.

- On the General Journals list page, select the OPENING journal.

- Open the assist edit button to the right of the Batch Name field.

- Select the CUST journal batch.

- Select OK.

Select the first line and fill in the following details. 
Enter 10/01/25 the Posting Date field 
Select Invoice in the Document type field

- Enter INV251001 in the Document No. field  
	Select Customer in the Account type field
	Enter 10000 in the Account No. field for Adatum Corporation
	Enter 1000 in the Amount field


Select a new line and fill in the following details. 
Enter 10/20/25 the Posting Date field  
Select Invoice in the Document type field

- Enter INV251002 in the Document No. field  
Select Customer in the Account type field
Enter 10000 in the Account No. field for Adatum Corporation
Enter 3600 in the Amount field

Select Home, Post

- Select Yes

- Select OK



- Open the assist edit button to the right of the Batch Name field.

- Select the VEND journal batch.

- Select OK.

- Using Personalization add field External Document No. General Journals page.

Select the first line and fill in the following details. 
Enter 10/10/25 the Posting Date field 
Select Invoice in the Document type field

Enter 25-034 in the Document No. field

Enter 25-034 in the External Document No. field    
Select Vendor in the Account type field
Enter 10000 in the Account No. field for Fabrikam, Inc.
Enter -5000 in the Amount field


Select a new line and fill in the following details. 
Enter 10/10/25 the Posting Date field  
Select Invoice in the Document type field

Enter 25-356 in the Document No. field

Enter 25-356 in the External Document No. field    
Select Vendor in the Account type field
Enter 10000 in the Account No. field for Fabrikam, Inc.
Enter -3600 in the Amount field


- Select Home, Post

- Select Yes

- Select OK


- Open the assist edit button to the right of the Batch Name field.

- Select the BANK journal batch.

- Select OK.


Select the first line and fill in the following details. 
Enter 12/31/25 the Posting Date field 
Select the empty option in the Document type field

Enter OPENBAL2 in the Document No. field  
	Select Bank in the Account type field
	Enter CHECKING in the Account No. field
	Enter 20495.87 in the Amount field
	Select 10100 Bank Account – Operating in the Balance Account No. field

- Select Home, Post

- Select Yes

- Select OK



## Task 2: Reverse posted entries: reverse register, reverse transaction.


## Scenario
You are working on opening balances for the Contoso company. Some entries posted as open balance transactions must be corrected. You need to cancel the following entries:


Customer detailed balances:


| Account no. | Account name | Document Date | Document No. | Amount, $ |
| --- | --- | --- | --- | --- |
| 10000 | Adatum Corporation | 10/20/25 | INV251002 | 3600 |


| Account no. | Account name | Document Date | Document No. | Amount, $ |
| --- | --- | --- | --- | --- |
| 10000 | Fabrikam, Inc. | 10/10/25 | 25-034 | -5000 |
| 10000 | Fabrikam, Inc. | 10/20/25 | 25-356 | -3600 |

You will perform:

- Reverse a transaction.

- Reverse register.


### Steps
1. Reverse a transaction.

Select the Search icon in the top-right corner of the page, enter Find entries and then choose the related link.
	Enter INV251002 in the Document No. field
	Enter 10/20/25 the Posting Date field
	Select Find
	Select G/L Entry line and select Show Related Entries.


On the General Ledger Entries page select Reverse Transaction
		On the Reverse Transaction Entries page select Reverse
		Select Yes
		Select OK.


2. Reverse register.

3. Select the Search icon in the top-right corner of the page, enter G/L Register and then choose the related link.
On the G/L Registers page, sort lines by No. field, Descending.
Select third line with Journal Batch name – VEND.
Select Vendor Ledger Entries to check entries in the register. 
Register has entries with Document no: 25-034, 25-356.

4. Close Vendor Ledger Entries page.

5. Select Reverse, Reverse Register.

6. On the Reverse Register Entries page, select Reverse.

7. Select Yes.
Select OK.



## Task 3: Utilize general ledger allocations


## Scenario
Contoso allocates shared operating expenses—such as utilities, insurance, and administrative overhead—across multiple departments to ensure accurate cost reporting. As the Financial Accountant, you are responsible for setting up and applying these allocation rules.

For this task, management has asked you to configure an allocation for Health Insurance expenses. The cost must be distributed across departments using the following proportions:

- Administrative Department: 25%

- Production Department: 25%

- Sales Department: 50%

After setting up the allocation rule, you must post an incoming invoice to apply it. Contoso has received invoice INV02
345 from Purchasing Inc. dated 2/1/26 for $1,200 representing the monthly health insurance cost.

You will perform:

- Set up an Allocation account.

- Create and post a purchase invoice for an allocation account.


### Steps
1. Set up an Allocation account.


Select the Search icon in the top-right corner of the page, enter Allocation Accounts and then choose the related link.
	Select +New and fill the fields on Allocation Account page:

Enter HEALTH in the No, field
	Enter Health Insurance in the Name field
	Select the Fixed in the Account type field.

Select the Split Amount in the Document line split field.

In the lines sections select for the first line:
	Select the G/L Account in the Destination Account type field
	Enter 73100 in the Destination Account number field
	Enter 25 to the Share field.
	Select Dimensions, Dimension code – DEPARTMENT, Dimension Value – ADM
	Select Close.
	In the new line:
	Select the G/L Account in the Destination Account type field
	Enter 73100 in the Destination Account number field
	Enter 25 to the Share field.
	Select Dimensions, Dimension code – DEPARTMENT, Dimension Value – PROD
	Select Close.
	
	In the new line:
	Select the G/L Account in the Destination Account type field
	Enter 73100 in the Destination Account number field
	Enter 25 to the Share field.
	Select Dimensions, Dimension code – DEPARTMENT, Dimension Value – PROD
	Select Close.
	Close Allocation Account card.


2. Create and post a purchase invoice for an allocation account.


Select the Search icon in the top-right corner of the page, enter Purchase Invoices, and then choose the related link.

In the Purchase Invoices list page, select + New.

On the General FastTab, fill in the following fields:

Enter V9001 In the Vendor No field with Vendor name Purchasing Inc.

In the Posting Date and Document Date fields, enter 2/1/26.

In the Vendor Invoice No. field, enter INV02-345

On the Lines section fill the first line:
	In the Type field, select Allocation Account
	In the No. field, select HEALTH
	Enter 1 in the Quantity field
	Entrer 1200 in the Amount field.

3. Select Post.

4. Select Yes to post.

5. Select No to open the posted invoice.