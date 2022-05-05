---
lab:
    title: 'Lab: Configure Chart of Accounts'
    module: 'Module 3: Configure Financials'
---

Hands-on-Lab 3.2: Configure Chart of Accounts
=============================================

Exercise 1: Configure the Chart of Accounts
-------------------------------------------

### Scenario

During the implementation process, Contoso’s superusers are systematically
informed and trained in different areas of the system during work sessions.
After following the work sessions about the chart of accounts, posting groups
and dimensions, the accounting manager has reviewed Contoso’s chart of accounts
and has added some g/l accounts.

Some accounts were added to distinguish very easily between purchases and sales
made within their own country, and for each product type, without having to set
up even more dimensions. These accounts will be posted to through the set up of
posting groups, which will be setup later in collaboration with you, the
functional consultant.

Also the expenses are more detailed, where we can see a clear separation between
staff-related expenses and other expenses. All staff-related expenses are posted
to the g/l accounts 60700 until 61100, where it is obligated to indicate a
specific department each time an expense is made. These departments will be
setup as a dimension, which will be done later on.

![](https://github.com/MicrosoftLearning/MB-800-Business-Central-Functional-Consultant/blob/master/Instructions/Labs/media/MB800_2021_Lab%203.2_chart_of_accounts.png)

Your first job is to make sure the g/l accounts are created correctly.

*Remark: for the income statement accounts, make sure to fill in the Tax Group
Code with the NONTAXABLE value. This is due to the use of a US-database.*

### Tasks

1.  Create a G/L Account card.

### Steps

1.  Create a G/L Account card.

    1.  In the **Chart of Accounts** page, select **New**.

    2.  In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘10250’

        2.  In the **Name** field, enter ‘European bank’.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Assets**

        5.  In the **Account Subcategory** field, enter the value **Cash**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    3.  In the **Chart of Accounts** page, select **New**.

    4.  In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘10450’

        2.  In the **Name** field, enter ‘Accounts Receivables – Foreign’.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Assets**

        5.  In the **Account Subcategory** field, enter the value **Accounts
            Receivables**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    6.  In the **Chart of Accounts** page, select **New**.

    7.  In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘10710’

        2.  In the **Name** field, enter ‘Inventory – Computer Hardware’.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Assets**

        5.  In the **Account Subcategory** field, enter the value **Inventory**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    8.  In the **Chart of Accounts** page, select **New**.

    9.  In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘20150’

        2.  In the **Name** field, enter ‘Accounts Payable – Foreign’.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Liabilities**

        5.  In the **Account Subcategory** field, enter the value **Current
            Liabilities**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    11. In the **Chart of Accounts** page, select **New**.

    12. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘40210’

        2.  In the **Name** field, enter ‘Product Sales – Computer Hardware’.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Income**

        5.  In the **Account Subcategory** field, enter the value **Income
            Product Sales**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Tax Group Code** field under the **Posting**, enter **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    13. In the **Chart of Accounts** page, select **New**.

    14. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘50150’

        2.  In the **Name** field, enter ‘Materials – Computer Hardware’.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Cost of Goods
            Sold**

        5.  In the **Account Subcategory** field, enter the value **Materials**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Tax Group Code** field under the **Posting**, enter **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    15. In the **Chart of Accounts** page, select **New**.

    16. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘61450’

        2.  In the **Name** field, enter ‘Travel Expenses.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Expense**

        5.  In the **Account Subcategory** field, enter the value **Utilities
            Expense**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Tax Group Code** field under the **Posting**, enter **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    17. In the **Chart of Accounts** page, select **New**.

    18. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter ‘61850’

        2.  In the **Name** field, enter ‘VAT’.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Expense**

        5.  In the **Account Subcategory** field, enter the value **Tax
            Expenses**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Tax Group Code** field under the **Posting**, enter **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    19. In the **Chart of Accounts** page, select **Process** and then select
        **Indent Chart of Accounts**.

    20. Click **Yes**.
