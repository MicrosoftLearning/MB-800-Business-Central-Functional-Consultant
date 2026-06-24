---
lab:
  title: 'Lab 22: Configure Copilot and agent capabilities'
  module: 'Invoicing customers in Dynamics 365 Business Central'
  duration: 30 minutes
  level: 300
  islab: true
---


## Exercise 22: Configure Copilot and agent capabilities


## Task 1: Activate and deactivate features

## Scenario
As the Business Central administrator, you need to adjust which Copilot features are available in Contoso environment. Your task is to activate features:

- Autofill fields

- Marketing text suggestions

- Suggest lines on sales documents with Copilot

- No. series suggestions

and deactivate the E
document matching assistance features your organization doesn’t plan to use for now.

### Steps
Select the Search icon in the top-right corner of the page, enter Copilot & agent capabilities, and then choose the related link.

In the  Copilot & agent capabilities page, 
	Select line with E
document matching assistance.
	Select Deactivate, select the Reason for deactivating – Users are not ready for it yet.

Check that lines have  the Active status in the Status field for:
	Autofill fields,
	Marketing text suggestions, 
	Suggest lines on sales documents with Copilot,
	No. series suggestions.

## Task 2: Granting access to Copilot features for users.

## Scenario
Once the features are configured, you’ll move on to assigning access. Every user need Copilot capabilities, so your task is to grant permissions for user to have access to the Autofill fields, Marketing text suggestions, Suggest lines on sales documents with Copilot and No. series suggestions features.
You will perform:

- Create a new Security group.

- Create a new Permission set.

- Assign permissions for the Security group.

### Steps
1. Create a new Security group.

Select the Search icon in the top-right corner of the page, enter Security Groups and then choose the related link.

Select +New.
On the New Security group page fill the fields:

In the Microsoft Intra security group name, select the All users group.
The field Code is auto populated.
Select Create.

2. Create a new Permission Set.

3. Select the Search icon in the top-right corner of the page, enter Permission Sets and then choose the related link

4. Select +New.

5. In the Permission Set field, enter COPILOT ADD

In the Name field, enter Copilot additional permissions.

Select Permissions.
	On the Permissions section select for new line:

In the Type field, select Include.
	In the Object Type field, select Page.
	In the Object ID field, enter 5836 (Copilot Marketing Text).
	section select for new line:

In the Type field, select Include.
	In the Object Type field, select Page.
	In the Object ID field, enter 7275 (Sales Line AI Suggestions).

section select for new line:

In the Type field, select Include.
	In the Object Type field, select Page.
	In the Object ID field, enter 7276 (Sales Line AI Suggestions Sub).

Close the Permission Set page.


6. Assign permissions for the Security group.

Select the Search icon in the top-right corner of the page, enter Security Groups and then choose the related link.

On the Security group page select the line for All users group

Select Permissions.

On the Security group permission sets page

In the new line select Permission Set field, enter COPILOT SYS FEATURES.
In the next line select Permission Set field, enter COPILOT ADD.

Close Security group permission sets page.
	Close Security group page.

## Task 3: Enable Bing Search for Copilot features.

## Scenario
Contoso wants to use the Autofill fields tool. To enable Copilot to get information from the web, you must set up the Enable Bing Search.

### Steps
Select the Search icon in the top-right corner of the page, enter Copilot & agent capabilities, and then choose the related link.
	In the Copilot & agent capabilities page,
	Activate Enable Bing Search.



