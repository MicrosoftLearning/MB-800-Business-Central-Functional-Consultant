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

Exercise 1: Configure the Chart of Accounts
-------------------------------------------

### Scenario

During the implementation process, Contoso’s superusers are systematically
informed and trained in different areas of the system during work sessions.
After following the work sessions about the chart of accounts, posting groups
and dimensions, the accounting manager has reviewed Contoso’s chart of accounts
and has added some g/l accounts. The further setup of posting groups is done in
collaboration with you, the functional consultant.

Some accounts were added to distinguish very easily between purchases and sales
made within their own country, and for each product type, without having to set
up even more dimensions. These accounts will be posted to through the setup of
posting groups.

Also the expenses are more detailed, where we can see a clear separation between
staff-related expenses and other expenses. All staff-related expenses are posted
to the g/l accounts 60700 until 61100, where it is obligated to indicate a
specific department each time an expense is made.


![](https://github.com/MicrosoftLearning/MB-800-Business-Central-Functional-Consultant/blob/master/Instructions/Labs/media/MB800_2021_Lab%203.2_chart_of_accounts.png)

Your first job is to make sure the g/l accounts are created correctly and that
the necessary dimensions are connected.

*Remark: for the income statement accounts, make sure to fill in the Tax Group
Code with the NONTAXABLE value.*

### Tasks

1.  Create a G/L Account card.

2.  Assign default dimensions to multiple G/L Accounts.

### Steps

1.  Create a G/L Account card.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Chart of Accounts**, and then choose the related link.

    2.  In the **Chart of Accounts** page, select **+ New**.

    3.  In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **10250**

        2.  In the **Name** field, enter **European bank**.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Assets**

        5.  In the **Account Subcategory** field, enter the value **Cash**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    4.  In the **Chart of Accounts** page, select **+ New**.

    5.  In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **10450**

        2.  In the **Name** field, enter **Accounts Receivables – Foreign**.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Assets**

        5.  In the **Account Subcategory** field, enter the value **Accounts
            Receivables**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    6.  Repeat steps c and d for account **10475**.

    7.  In the **Chart of Accounts** page, select **+ New**.

    8.  In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **10710**

        2.  In the **Name** field, enter **Inventory – Computer Hardware**.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Assets**

        5.  In the **Account Subcategory** field, enter the value **Inventory**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    9.  In the **Chart of Accounts** page, select **+ New**.

    10. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **20150**

        2.  In the **Name** field, enter **Accounts Payable – Foreign**.

        3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

        4.  In the **Account Category** field, enter the value **Liabilities**

        5.  In the **Account Subcategory** field, enter the value **Current
            Liabilities**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  Close the **G/L Account Card** page.

    11. Repeat steps h and i for the account **20175**.

    12. In the **Chart of Accounts** page, select **+ New**.

    13. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **40210**

        2.  In the **Name** field, enter **Product Sales – Computer hardware**.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Income**

        5.  In the **Account Subcategory** field, enter the value **Income
            Product Sales**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Posting** FastTab, in the **Tax Group Code** field, enter
            **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    14. In the **Chart of Accounts** page, select **+ New**.

    15. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **50150**

        2.  In the **Name** field, enter **Materials - Computerhardware**.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Cost of Goods
            Sold**

        5.  In the **Account Subcategory** field, enter the value **Materials**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Posting** FastTab, in the **Tax Group Code** field, enter
            **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    16. In the **Chart of Accounts** page, select **+ New**.

    17. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **61450**

        2.  In the **Name** field, enter **Travel Expenses**.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Expense**

        5.  In the **Account Subcategory** field, enter the value **Utilities
            Expense**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Posting** FastTab, in the **Tax Group Code** field, enter
            **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    18. In the **Chart of Accounts** page, select **+ New**.

    19. In the new general ledger account card, fill in the following fields:

        1.  In the **No.** field, enter **61850**

        2.  In the **Name** field, enter **VAT**.

        3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

        4.  In the **Account Category** field, enter the value **Expense**

        5.  In the **Account Subcategory** field, enter the value **Tax
            Expenses**.

        6.  Deselect the **Direct Posting** checkbox.

        7.  In the **Posting** FastTab, in the **Tax Group Code** field, enter
            **NONTAXABLE**.

        8.  Close the **G/L Account Card** page.

    20. In the **Chart of Accounts** page, select **Process** and then select
        **Indent Chart of Accounts**.

    21. Click **Yes**.

2.  Assign default dimensions to multiple G/L Accounts.

    1.  In the **Chart of Accounts** page, select general ledger accounts 60700
        until 61100.

    2.  Select **Account**, then **Dimensions-Multiple**, and then select
        **Dimensions – Multiple**.

    3.  In the **Default Dimensions-Multiple** page, select **+ New**.

    4.  In the **Dimensions Code** field, enter **DEPARTMENT**.

    5.  In the **Value Posting** field, enter the value **Code Mandatory**.

    6.  Click **OK**.
