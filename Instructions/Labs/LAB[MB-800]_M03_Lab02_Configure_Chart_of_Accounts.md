---
lab:
    title: 'Lab: Configure Chart of Accounts and Posting Groups'
    module: 'Module 3: Configure Financials'
---

## Exercise 1: Configure the Chart of Accounts

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

![Chart of Accounts](media/lab3_2_chart_of_accounts.png)

Your first job is to make sure the g/l accounts are created correctly and that
the necessary dimensions are connected.

***Remark: for the income statement accounts, make sure to fill in the Tax Group
Code with the NONTAXABLE value.***

### Tasks

1.  Create a G/L Account card.

2.  Assign default dimensions to multiple G/L Accounts.

### Steps

1.  Create a G/L Account card.

2.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **Chart of Accounts** and click the **Chart of Accounts** link. 

3.  In the **Chart of Accounts** page, select **New**.

4.  In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘10250’

      2.  In the **Name** field, enter ‘European bank’.

      3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

      4.  In the **Account Category** field, enter the value **Assets**

      5.  In the **Account Subcategory** field, enter the value **Cash**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  Close the **G/L Account Card** page.

5.  In the **Chart of Accounts** page, select **New**.

6.  In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘10450’

      2.  In the **Name** field, enter ‘Accounts Receivables – Foreign’.

      3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

      4.  In the **Account Category** field, enter the value **Assets**

      5.  In the **Account Subcategory** field, enter the value **Accounts
            Receivables**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  Close the **G/L Account Card** page.

7.  Repeat steps c and d for the account ‘10475’.


8.  In the **Chart of Accounts** page, select **New**.

9.  In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘10710’
      
      2.  In the **Name** field, enter ‘Inventory – Computer Hardware’.

      3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

      4.  In the **Account Category** field, enter the value **Assets**

      5.  In the **Account Subcategory** field, enter the value **Inventory**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  Close the **G/L Account Card** page.


10. In the **Chart of Accounts** page, select **New**.

11. In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘20150’

      2.  In the **Name** field, enter ‘Accounts Payable – Foreign’.

      3.  In the **Income/Balance** field, enter the value **Balance Sheet**.

      4.  In the **Account Category** field, enter the value **Liabilities**

      5.  In the **Account Subcategory** field, enter the value **Current
            Liabilities**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  Close the **G/L Account Card** page.

12. Repeat steps h and i for the account ‘20175’.

13. In the **Chart of Accounts** page, select **New**.

14. In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘40210’

      2.  In the **Name** field, enter ‘Product Sales – Computer hardware’.

      3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

      4.  In the **Account Category** field, enter the value **Income**

      5.  In the **Account Subcategory** field, enter the value **Income
            Product Sales**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  *In the* **Tax Group Code** *field, enter NONTAXABLE.*

      8.  Close the **G/L Account Card** page.

15. In the **Chart of Accounts** page, select **New**.

16. In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘50150’

      2.  In the **Name** field, enter ‘Materials - Computerhardware’.

      3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

      4.  In the **Account Category** field, enter the value **Cost of Goods
            Sold**

      5.  In the **Account Subcategory** field, enter the value **Materials**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  *In the* **Tax Group Code** *field, enter NONTAXABLE.*

      8.  Close the **G/L Account Card** page.

17. In the **Chart of Accounts** page, select **New**.

18. In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘61450’

      2.  In the **Name** field, enter ‘Travel Expenses.

      3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

      4.  In the **Account Category** field, enter the value **Expense**

      5.  In the **Account Subcategory** field, enter the value **Utilities
            Expense**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  *In the* **Tax Group Code** *field, enter NONTAXABLE.*

      8.  Close the **G/L Account Card** page.

19. In the **Chart of Accounts** page, select **New**.

20. In the new general ledger account card, fill in the following fields:

      1.  In the **No.** field, enter ‘61850’

      2.  In the **Name** field, enter ‘VAT’.

      3.  In the **Income/Balance** field, enter the value **Income
            Statement**.

      4.  In the **Account Category** field, enter the value **Expense**

      5.  In the **Account Subcategory** field, enter the value **Tax
            Expenses**.

      6.  Deselect the **Direct Posting** checkbox.

      7.  *In the* **Tax Group Code** *field, enter NONTAXABLE.*

      8.  Close the **G/L Account Card** page.

21. In the **Chart of Accounts** page, select **Process** and then select
    **Indent Chart of Accounts**.

22. Click **Yes**.

23. Assign default dimensions to multiple G/L Accounts.

24. In the **Chart of Accounts** page, select general ledger accounts 60700
    until 61100.

25. Select **Related**, then **Account**, then **Dimensions** and then
    select **Dimensions – Multiple**.

26. In the **Default Dimensions-Multiple** page, select **New**.

27. In the **Dimensions Code** field, enter DEPARTMENT.

28. In the **Value Posting** field, enter the value **Code Mandatory**.

29. Click **OK**.

## Exercise 2: Set up posting groups

### Scenario

Contoso recently decided to start selling computer hardware through their
European web shop. To keep track of these new line of product, they will record
these sales on a separate income statement account 40210, apart from the other
retail activities. They will have to comply to European legislation and
calculate 15% VAT on all their web shop sales. This VAT amount will be posted to
the general ledger account 61850. *(Remark: this is just for exercise purposes
and not based on actual legislation.)*

The products are mainly purchased with export vendors, no VAT needs to be paid
in these countries. Purchase with EU vendors is however also possible.

The necessary general ledger accounts were already created in the previous
exercise. It is now up to you to complete the General Posting Setup and the VAT
Posting Setup.

### Tasks

1.  Create a VAT Product Posting Group.

2.  Create a VAT Business Posting Group.

3.  Complete the Tax Posting Setup.

4.  Create a Product Posting Group.

5.  Create a Business Posting Group.

6.  Complete the General Posting Setup.

### Steps

1.  Create a VAT Product Posting Group.

2.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **VAT Product Posting Groups**, then click the link **VAT Product Posting Groups**.

3.  In the **VAT Product Posting Groups** page, select **New**.

4.  In the **Code** field, enter G15.

5.  In the **Description** field, enter ‘Goods 15%’.

6.  Create a VAT Business Posting Group.

7.  In the **VAT Business Posting Groups** page, select **New**.

8.  In the **Code** field, enter EU.

9.  In the **Description** field, enter ‘EU’.

10. Complete the Tax Posting Setup.

11. In the **Tax Posting Setup** page, select **New**.

12. In the new tax posting setup card, fill in the following fields:

      1.  In the **VAT Bus. Posting Group** field, enter EU.

      2.  In the **VAT Prod. Posting Group** field, enter G15.

      3.  In the **VAT Calculation Type** field, enter Normal Tax.

      4.  In the **Description** field, enter ‘web shop sales’.

      5.  In the **Tax%** field, enter 15.

      6.  In the **Tax Identifier** field, enter G15.

      7.  In the Sales Tax Account field, enter 61850.

13. Create a Product Posting Group.

14. In the **General Product Posting Groups** page, select **New**.

15. In the **Code** field, enter COMPUTERHW.

16. In the **Description** field, enter ‘computer hardware’.

17. In the **Def. VAT Prod. Posting Group** field, enter G15.

18. Create a Business Posting Group

19. In the **Gen. Business Posting Groups** page, select **New**.

20. In the **Code** field, enter EU.

21. In the **Description** field, enter ‘EU customer and vendors’.

22. In the **Def. VAT Bus. Posting Group** field, enter EU.

23. In the **Gen. Business Posting Groups** page, select **New**.

24. In the **Code** field, enter EXPORT.

25. In the **Description** field, enter ‘Export customer and vendors’.

26. Leave the **Def. VAT Bus. Posting Group** field blank.

27. Complete the General Posting Setup.

28. In the **General Posting Setup** page, select **New**.

29. In the new general posting setup card, in the **General** FastTab, fill in the following fields:

      1.  In the **Gen. Bus. Posting Group** field, fill in EU.

      2.  In the **Gen. Prod. Posting Group** field, fill in COMPUTERHW.

30. Select **Copy**.

31. In the page that opens, fill in the following fields:

      1.  In the **Gen. Bus. Posting Group** field, fill in DOMESTIC.
      
      2.  In the **Gen. Prod. Posting Group** field, fill in RETAIL.

      3.  In the **Copy** field, select the **All fields** option.

      4.  Leave all the checkboxes selected.

      5.  Click **OK**.

32. In the new general posting setup card, in the **Sales** FastTab, change the following fields:

      1.  In the **Sales Account** field, change 40200 to 40210

      2.  In the **Sales Credit Memo Account** field, change 40200 to 40210

33. In the new general posting setup card, in the **Purchases** FastTab, change the following fields:

      1.  In the **Purch. Account** field, change 10700 to 50150.

      2.  In the **Purch. Credit Memo Account** field, change 10700 to 50150.

34. In the **General Posting Setup** page, select **New**.

35. In the new general posting setup card, in the **General** FastTab, fill in the following fields:

      1.  In the **Gen. Bus. Posting Group** field, fill in EXPORT.

      2.  In the **Gen. Prod. Posting Group** field, fill in COMPUTERHW.
       
36. Select **Copy**.

37. In the page that opens, fill in the following fields:

      1.  In the **Gen. Bus. Posting Group** field, fill in EU.

      2.  In the **Gen. Prod. Posting Group** field, fill in COMPUTERHW.

      3.  In the **Copy** field, select the **All fields** option.

      4.  Leave all the checkboxes selected.

      5.  Click **OK**.
