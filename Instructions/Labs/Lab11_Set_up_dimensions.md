---
lab:
  title: 'Lab 11: Set up dimensions'
  module: 'Set up dimensions in Dynamics 365 Business Central'
  duration: 45 minutes
  level: 300
  islab: true
---

## Exercise 11: Set up dimensions

## Task 1: Set up a dimension with dimension values

## Scenario
Contoso has expressed their requirements regarding reporting goals.

From the general ledger they would like to analyze their sales by sales person and customer group.

They want to see both the income and the discounts granted for each sales person.

A dimension for the customer group already exists, but it is up to you to create a dimension for sales people as well.

You will perform -

1. Set up a dimension with dimension values

### Steps
1. Set up a dimension with dimension values
   1. Select the Search icon in the top-right corner of the page, enter Dimensions, and then choose the related link.
   2. In the **Dimensions** page, select **+ New**.
   3. In the **Code** field, enter CUSTOMERGROUP.
   4. Select **Dimension** and then **Dimension Values**.
   5. For each sales person, enter the initials in the **Code** field and the full name in the **Name** field.
      1. LARGE - Large Business
      2. MEDIUM - Medium Business
      3. SMALL - Small Business
   6. Check that each dimension value line is set the **Dimension Value Type** field to the **Standard** value.

## Task 2:

Assign Account Type Default Dimensions

## Scenario
To keep their analytical information as consistent as possible they would like to make sure that Business Central obligates the user to enter dimension information when posting sales transactions.

Every time a sales transaction is registered the customer’s group should be added and the salesperson’s code should be entered.

When a new customer is created, they are categorized to a certain group, which will be evaluated on a yearly basis. The customer, however, can be serviced by different salespeople responsible for their customer group.

You will perform -

1. Assign Account Type Default Dimensions for the customer group.
2. Assign Account Type Default Dimensions for the sales people.

### Steps
1. Assign Account Type Default Dimensions for the customer group.
   1. In the **Dimensions** page, select the **CUSTOMERGROUP** dimension.
   2. Select **Dimension**, and then select **Account Type Default Dim.**.
   3. On a new line, open the assist edit button to the right of the **Table ID** field.
   4. In the window that opens, select the **Customer** table (Table ID 18) and select **OK**.
   5. In the **Value Posting** field, enter **Code Mandatory**.
2. Assign Account Type Default Dimensions for the sales people.
   1. In the **Dimensions** page, select the **SALESPERSON** dimension.
   2. Select **Dimension**, and then select **Account Type Default Dim.**.
   3. Open the assist edit button to the right of the **Table ID** field.
   4. In the window that opens, select the **Salesperson/Purchaser** table (Table ID 13), and select **OK**.
   5. In the **Value Posting** field, enter **Code Mandatory**.

## Task 3: Set up a dimension combination

## Scenario
Sales people are divided into sales teams, where each team is responsible for a specific customer group.

To further enhance the accuracy of their analytical information, you have to make sure only logical dimension combination can be made when posting sales transactions.

Make sure the following requirements are met:

* The sales team for the small businesses consists of the following people:
  + Annette Hill
  + Bart Duncan
* The sales team for the medium sized customers consists of the following people:
  + Debra L. Core
  + John Roberts
* The sales team for large companies consists of the following people:
  + Mary A. Dempsey
  + Peter Saddow
  + Richard Lum

You will perform -

1. Limit a dimension combination.
2. Block dimension value combinations.

### Steps
1. Limit a dimension combination.
   1. Select the Search icon in the top-right corner of the page, enter Dimension Combinations, and then choose the related link.
   2. In the **Dimension Combinations** page, select the **CUSTOMERGROUP** row, and select on the **SALESPERSON** row in the dimension matrix.

In the window that opens, select **Limited**.

1. Select **OK**.

1. Block dimension value combinations.
   1. In the **Dimension Combinations** page, select on the **Limited** value of the combination of the **CUSTOMERGROUP** and **SALESPERSON** dimension in the matrix.
   2. Select **Yes** to view the list of values.
   3. Select on the combination of the AH and MEDIUM dimension values in the matrix.
   4. In the window that opens, select **Blocked**.
   5. Select **OK**.
   6. Repeat steps 3. 4. and 5., for the following combinations:
      1. AH – LARG
      2. BD – MEDIUM
      3. BD – LARGE
      4. DC – SMALL
      5. DC – LARGE
      6. JR – SMALL
      7. JR – LARGE
      8. MD – SMALL
      9. MD – MEDIUM
      10. PS – SMALL
      11. PS – MEDIUM
      12. RL – SMALL
      13. RL – MEDIUM

## Task 4: Set up global dimensions and shortcut dimensions

## Scenario
The company wants to easily identify the most important dimension **BUSINESSGROUP** and **DEPARTMENT** within every transaction and document. To support better analysis, the sales manager needs the ability to view both the **CUSTOMERGROUP** and **SALESPERSON** directly in the posted entries as well.

You will perform:

* Assing Global dimension.
  1. Assign Shortcut dimensions.Select the Search icon in the top-right corner of the page, enter **General Ledger Setup**, and then choose the related link.
  2. On the ribbon bar select Change Global Dimension.
  3. Select Global Dimension 1 Code – BUSINESSGROUP, Global Dimension 2 Code – DEPARTMENT.
  4. Select Sequential, Start.
  5. When process is done back to General Ledger Setup page and check that Global Dimension Code 1 field has value BUSINESSGROUP and Global Dimension Code 2 field – DEPARTMENT on in Dimensions section. Click Show more.
  6. Select Shortcut Dimension 3 as CUSTOMERGROUP and Shortcut Dimension 4 as SALESPERSON.

## Task 5: Set up default dimensions for master data

## Scenario
The company decided to implement CUSTOMERGROUP dimension. It is necessary to assign dimension values for an existing list of customers.

You will perform:

* Assign dimension value for multiple customers on the list.
* Assign specific dimension value for one customer card.

1. Select the Search icon in the top-right corner of the page, enter **Customers** and then choose the related link.
2. Click first three lines:
3. On the ribbon select Customer, Dimensions – Multiple, Dimensions – Multiple.
4. On the page Default Dimensions –Multiple click New and add new line with Dimension Code – CUSTOMERGROUP, Dimension Value Code – SMALL, Value Posting – Code Same Code.
5. Click OK.
6. Unselect all customers and click on the line with customer 50000 Relecloud.
7. On the ribbon bar select Customer, Dimensions-Multiple, Dimensions-Single,
8. In new line select Dimension Code – CUSTOMERGROUP, Dimension Value Code – LARGE, Value Posting – Same Code.

|  |
| --- |
| Repeat steps 7-8 for 40000 Alpine Ski House customer with Dimension Value Code - MEDIUM. |
|  |
|  |