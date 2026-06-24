---
lab:
  title: 'Lab 12: Prepare financial reporting'
  module: 'Configure financial reports in Dynamics 365 Business Central'
  duration: 30 minutes
  level: 200
  islab: true
---


## Exercise 12: Prepare financial reporting

## Task 1: Create new Account Category for G/L Acccount

## Scenario
Contoso is working to improve the quality and structure of its financial reporting in Business Central. During a review of the current setup, it becomes clear that several general ledger accounts are not assigned to Account Categories. As a result, these accounts do not appear correctly in the Income Statement report.

As the functional consultant responsible for financial configuration, you are tasked with updating the 50310 Project cost and 50320 Project Cost Applied accounts. This includes creating a new Account Category called “Project Cost”.

You will perform:

- Set up new account category

- Assign an account category to G/L Accounts


### Steps
1. Set up new account category

Select the Search icon in the top-right corner of the page, enter G/L Account Categories and then choose the related link.

On the G/L Account Categories list, select Edit list.

Select line with Job Cost description in the Cost of Goods Sold group.

2. Select New on the menu.

3. Enter Project Cost in the Description field.

4. Close G/L Account Categories.


5. Assign an account category to G/L Accounts

Select the Search icon in the top-right corner of the page, enter Chart of Accounts and then choose the related link.

In the Chart of Accounts page,

Select the line with G/L account 50310 Project Costs, select Edit.

Select the Project cost in the Account Subcategory field.

Select OK.

Close G/L Account card.

Select the line with G/L account 50320 Project Cost Applied, select Edit.

Select the Project cost in the Account Subcategory field.

Select OK.

Close G/L Account card.



## Task 2: Prepare financial reporting with Account Categories

## Scenario
After updating the chart of accounts and assigning Account Categories, Contoso is ready to 	improve how financial data is presented in reports. Management now expects financial statements to reflect the updated structure, including the newly introduced “Project Cost” category for better visibility of project-related expenses.

As the functional consultant, your next task is to prepare and validate financial reports based on Account Categories

### Steps
Select the Search icon in the top-right corner of the page, enter G/L Account Categories, and then choose the related link.

Select more, General Ledger Setup.

On the Reporting FastTab select More.
	In the Account Receivables G/L Account Category field, select 4 Accounts Receivables.

In the Account Payables G/L Account Category field, select 11 Current Liabilities.
	The Codes for reports that are auto populated.
	Close General Ledger Setup.


On the G/L Account Categories page, select Generate Financial Reports.
	Choose the Overwrite existing financial reports and row definitions option.

Select OK.

