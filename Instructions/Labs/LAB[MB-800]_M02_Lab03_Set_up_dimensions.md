---
lab:
    title: 'Lab: Set up dimensions'
    module: 'Module 2: Application Setup'
---

## Exercise 1: Set up a dimension with dimension values

### Scenario

Contoso has expressed their requirements regarding reporting goals.

From the general ledger they would like to analyze their sales by sales person
and customer group, using the following pivot-table:

![Pivot Table](media/lab2_3_pivot_table.png)

They want to see both the income and the granted discounts for each sales
person.

A dimension for the customer group already exists, but it is up to you to create
a dimension for sales people as well.

### Tasks

1.  Set up a dimension with dimension values

### Task 1: Set up a dimension with dimension values.
   
2.  From the main Business Central page in the black bar at the top of the page to the right, click the search icon. Type **Dimensions**, then select the **Dimensions** link.

4. In the **Dimensions** page, select **+ New**.

5.  In the **Code** field, enter SALESPERSON.

6.  Select **Dimension** in the menu bar and then **Dimension Values** (you may get an error message that this already exists. If this happens, select the SALESPERSON row value to continue).

7.  For each sales person, enter the initials in the **Code** field and the full name in the **Name** field.

    -   AH - Annette Hill

    -   BD - Bart Duncan

    -   DC - Debra L. Core

    -   JR - John Roberts

    -   MD - Mary A. Dempsey

    -   PS - Peter Saddow

    -   RL - Richard Lum

8.  For each sales person, set the **Dimension Value Type** field to the
    **Standard** value.

    **Note:** To save you will need to click into a new field. You can see saved status in the upper right corner.

## Exercise 2: Assign Account Type Default Dimensions

### Scenario

To keep their analytical information as consistent as possible they would like
to make sure that Business Central obligates the user to enter dimension
information when posting sales transactions.

Every time a sales transactions is registered the customer’s group should be
added and the sales person’s code should be entered.

When a new customer is created they are categorized to a certain group, which
will be evaluated on a yearly basis. The customer however can be serviced by
different sales people responsible for their customer group.

### Tasks

1.  Assign Account Type Default Dimensions for the customer group.

2.  Assign Account Type Default Dimensions for the sales people.

### Task 1: Assign Account Type Default Dimensions for the customer group.

1.  Navgate back to the **Dimensions** page using the search function in the black bar at the top of the page on the right hand side.

3.  In the **Dimensions** page, select the CUSTOMERGROUP dimension.

4.  Select **Dimension**, and then select **Account Type Default Dim.**.

5.  Open the assist edit button to the right of the **Table ID** field.

6.  In the window that opens, select the **Customer** table and click
    **OK**.

7.  In the **Value Posting** field, enter **Code Mandatory**.

### Task 2: Assign Account Type Default Dimensions for the sales people.

1.  In the **Dimensions** page, select the SALESPERSON dimension.

10. Select **Dimension**, and then select **Account Type Default Dim.**.

11. Open the assist edit button to the right of the **Table ID** field.

12. In the window that opens, select the **Salesperson/Purchaser** table and
    click **OK**.

13. In the **Value Posting** field, enter **Code Mandatory**.

## Exercise 3: Set up a dimension combination

### Scenario

Sales people are divided into sales teams, where each team is responsible for a
specific customer group.

To further provide enhance the accuracy of their analytical information, you
have to make sure only logical dimension combination can be made when posting
sales transactions.

Make sure the following requirements are met:

-   The sales team for the small businesses consists of the following people:

    -   Annette Hill

    -   Bart Duncan

-   The sales team for the medium sized customers consists of the following
    people:

    -   Debra L. Core

    -   John Roberts

-   The sales team for large companies consists of the following people:

    -   Mary A. Dempsey

    -   Peter Saddow

    -   Richard Lum

### Tasks

1.  Limit a dimension combination.

2.  Block dimension value combinations.

### Task 1: Limit a dimension combination.

1.  From the main Business Central page in the black bar at the top of the page to the right, click the search icon. Type **Dimension Combinations**, then select the **Dimension Combinations** link.

3.  In the **Dimension Combinations** page, click to select the CUSTOMERGROUP dimension, and then also click to select the SALESPERSON dimension in the matrix.

4.  In the window that opens, select **Limited**.

### Task 2: Block dimension value combinations.

6.  In the **Dimension Combinations** page, click on the **Limited** value
    of the combination of the CUSTOMERGROUP and SALESPERSON dimension in the
    matrix.

7.  Click **Yes**.

8.  Click on the combination of the AH and MEDIUM dimension values in the
    matrix.

9.  In the window that opens, select **Blocked**.

10. Repeat steps c. and d., for the following combinations:

    -   AH – LARG

    -   BD – MEDIUM

    -   BD – LARGE

    -   DC – SMALL

    -   DC – LARGE

    -   JR – SMALL

    -   JR – LARGE

    -   MD – SMALL

    -   MD – MEDIUM

    -   PS – SMALL

    -   PS – MEDIUM

    -   RL – SMALL

    -   RL – MEDIUM
