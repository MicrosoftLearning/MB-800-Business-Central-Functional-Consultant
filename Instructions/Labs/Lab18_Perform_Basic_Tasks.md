---
lab:
  title: 'Lab 18: Perform Basic tasks in Business Central'
  module: 'User interface essentials in Dynamics 365 Business Central'
  duration: 30 minutes
  level: 200
  islab: true
---


## Exercise 18: Perform Basic tasks in Business Central


## Task 1: Customize page in the existing user Profile.

## Scenario
Contoso has implemented a sales manager for customers. Each customer has one salesperson. The sales director has expressed the following requirements:


All sales managers will use the same Profile – SALES MANAGER in the system. They need to see the same view of the Customer list with the following fields:


- No.

- Name

- Location Code

- Salesperson Code

- Phone No.

- Contact

- Credit Limit(LCY)

- Balance(LCY)

- OverDue Balance(LCY)

- Sales(LCY)

- Payments(LCY)


### Steps
1. Select the Search icon in the top-right corner of the page, enter Profiles(Roles) and then choose the related link.

2. In the Profiles(Roles) page, select line with Profile ID field – SALES MANAGER, select Manage, Edit on the menu.

3. Select Customize page.

4. NOTE: New web page will be opened in the browser in Customize mode, in the left top corner will be the sign Customizing, Sales Manager.


5. Select in the menu More, Customers, Open.

6. Select a line in the Customers section.

7. Select +Field on the menu.

8. Select fields one by one, click on the red triangle near the field name, select the option Hide for the following fields:

9. Responsibility Center

10. Allow multiple posting groups


11. Drag and drop one by one from Add to Field Section to the Customers section the following fields:

12. Salesperson Code

13. Credit Limit(LCY)


Select Done. Message Customization completed successfully. ... will be shown.


Close the current web page then return to the initial web page with the Sales Manager Profile open.

Select Enabled and Show in Role Explorer fields.



## Task 2: Personalize page.

## Scenario
Sales director wants to add additional fields for his own customer list screen:

- Country/Region Code

- Shipping Agent Code

- Payment terms Code


### Steps
1. Select the Search icon in the top-right corner of the page, enter Customers and then choose the related link.

2. Select Settings icon in the top-right corner of the page and select Personalize.

3. Select +Field and drag and drop one by one from Add to Field Section to the Customers section the following fields:

4. Country/Region Code

5. Shipping Agent Code

6. Payment terms Code

Select Done.


## Task 3: Configure Data Analysis mode.

## Scenario
The sales manager wants to see the customer sales by the salesperson on the customer list page.


### Steps
1. Select the Search icon in the top-right corner of the page, enter Customers and then choose the related link.

Select Enter Analysis mode on the menu ribbon.

Select + New Analysis view.

Enter Sales by Salespeople to the Name field, select OK.

Select Pivot mode field in the right section.

Select the Salesperson field.

Select the Name field.

Remove fields in the Values section: Credit Limit (LCY), Balance (LCY), Overdue Balance (LCY).





