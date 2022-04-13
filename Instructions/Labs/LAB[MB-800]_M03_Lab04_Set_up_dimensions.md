---
lab:
    title: 'Lab: Set up dimensions'
    module: 'Module 3: Configure Financials'
---

Hands-on-Lab 3.4: Set up dimensions
===================================

Exercise 1: Set up a dimension with dimension values
----------------------------------------------------

### Scenario

Contoso’s accounting manager has expressed their requirements regarding
reporting goals and analysis of recorded accounting data will be mainly focused
on the sales transactions.

From the general ledger they would like to analyze their sales by sales person
and customer group, using the following pivot-table:

![](https://github.com/MicrosoftLearning/MB-800-Business-Central-Functional-Consultant/blob/master/Instructions/Labs/media/MB800_2021_Lab%203.4_pivot_table.png)

They want to see both the income and the granted discounts for each sales
person.

Apart from the focus on sales analysis, Contoso’s accounting manager would also
like to track costs by department.

Dimensions for the customer group and department already exists, but it is up to
you to create a dimension for sales people as well.

*Remark: the dimensions SALESPERSON already exists in the demo database, but
this will be disregarded and a new dimension will be created*

### Tasks

1.  Set up a dimension with dimension values

### Steps

1.  Set up a dimension with dimension values

    1.  *In the Dimensions page:*

        1.  *Select the existing dimension SALESPERSON.*

        2.  *Select the Blocked checkbox.*

    2.  In the **Dimensions** page, select **New**.

    3. In the **Code** field, enter **SALESPEOPLE**.

    4.  Select **Dimension** and then **Dimension Values**.

    5.  For each sales person, enter the initials in the **Code** field and the
        full name in the **Name** field.

        -   AH - Annette Hill

        -   BD - Bart Duncan

        -   DC - Debra L. Core

        -   JR - John Roberts

        -   MD - Mary A. Dempsey

        -   PS - Peter Saddow

        -   RL - Richard Lum

    6.  For each sales person, set the **Dimension Value Type** field to the
        **Standard** value.

Exercise 2: Set up global dimensions and shortcut dimensions
------------------------------------------------------------

### Scenario

Since the analysis of recorded accounting data will be mainly focused on the
sales transactions, Contoso’s accounting manager would like to make analysis
directly from the chart of accounts, to make sure all the detailed information
is at hand.

He would also like to track costs by department where, for now, the main focus
is on easily entering this information. The specific reporting details will be
determined later on.

### Tasks

1.  Set up global dimensions.

2.  Set up shortcut dimensions.

### Steps

1.  Set up global dimensions.

    1.  In the **General Ledger Setup** page, select **Actions**, then
        **Functions** and then **Change Global Dimensions**.

    2.  In the **Change Global Dimensions** page, fill in the following fields:

        1.  In the **Global Dimension 1 Code** field select the value
            SALESPEOPLE.

        2.  In the **Global Dimension 2 Code** field leave the value
            CUSTOMERGROUP.

    3.  Select **Sequential** and then click **Start**.

    4.  Close the **Change Global Dimensions** page.

2.  Set up shortcut dimensions.

    1.  In the **General Ledger Setup** page, in the **Dimensions** FastTab, in
        the **Shortcut Dimension 3 Code** field select the value DEPARTMENT.

Exercise 3: Assign Account Type Default Dimensions
--------------------------------------------------

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

### Steps

1.  Assign Account Type Default Dimensions for the customer group.

    1.  In the **Dimensions** page, select the CUSTOMERGROUP dimension.

    2.  Select **Dimension**, and then select **Account Type Default Dim.**.

    3.  Open the assist edit button to the right of the **Table ID** field.

    4.  In the window that opens, select the **Customer** table and click
        **OK**.

    5.  In the **Value Posting** field, enter **Code Mandatory**.

2.  Assign Account Type Default Dimensions for the sales people.

    1.  In the **Dimensions** page, select the SALESPEOPLE dimension.

    2.  Select **Dimension**, and then select **Account Type Default Dim.**.

    3.  Open the assist edit button to the right of the **Table ID** field.

    4.  In the window that opens, select the **Salesperson/Purchaser** table and
        click **OK**.

    5.  In the **Value Posting** field, enter **Code Mandatory**.

Exercise 4: Assign default dimensions
-------------------------------------

### Scenario

Apart from the focus on sales analysis, Contoso’s accounting manager would also
like to track costs by department. This analytical information as well should be
kept as consistently as possible, by obligating the users to enter dimension
information when posting purchase cost transactions.

Expense accounts have already been set up more detailed. We can see a clear
separation between staff-related expenses and other expenses in the chart of
accounts. All staff-related expenses are posted to the g/l accounts 60700 until
61100, where it is obligated to indicate a specific department each time an
expense is made.

### Tasks

1.  Assign default dimensions to multiple G/L Accounts.

### Steps

1.  Assign default dimensions to multiple G/L Accounts.

    1.  In the **Chart of Accounts** page, select general ledger accounts 60700
        until 61100.

    2.  Select **Account**, and then select **Dimensions – Multiple**.

    3.  In the **Default Dimensions-Multiple** page, select **New**.

    4.  In the **Dimensions Code** field, enter DEPARTMENT.

    5.  In the **Value Posting** field, enter the value **Code Mandatory**.

    6.  Click **OK**.

Exercise 5: Set up a dimension combination
------------------------------------------

### Scenario

Sales people are divided into sales teams, where each team is responsible for a
specific customer group.

To further enhance the accuracy of their analytical information, you have to
make sure only logical dimension combination can be made when posting sales
transactions.

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

### Steps

1.  Limit a dimension combination.

    1.  In the **Dimension Combinations** page, click on the combination of the
        CUSTOMERGROUP and SALESPEOPLE dimension in the matrix.

    2.  In the window that opens, select **Limited**.

2.  Block dimension value combinations.

    1.  In the **Dimension Combinations** page, click on the **Limited** value
        of the combination of the CUSTOMERGROUP and SALESPEOPLE dimension in the
        matrix.

    2.  Click **Yes**.

    3.  Click on the combination of the AH and MEDIUM dimension values in the
        matrix.

    4.  In the window that opens, select **Blocked**.

    5.  Repeat steps c. and d., for the following combinations:

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
