
---
lab:
    title: 'Lab: Configure Posting Groups'
    module: 'Module 3: Configure Financials'
---

Hands-on-Lab 3.3: Configure Posting Groups
==========================================

Exercise 1: Set up posting groups
---------------------------------

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

*Remark: For exercise purposes, also create a Tax Posting Setup combination with
a blank VAT Product Posting Group and a blank VAT Business Posting Group.*

### Tasks

1.  Create a VAT Product Posting Group.

2.  Create a VAT Business Posting Group.

3.  Complete the Tax Posting Setup.

4.  Create a Product Posting Group.

5.  Create a Business Posting Group.

6.  Complete the General Posting Setup.

### Steps

1.  Create a VAT Product Posting Group.

    1.  In the **VAT Product Posting Groups** page, select **New**.

    2.  In the **Code** field, enter G15.

    3.  In the **Description** field, enter ‘Goods 15%’.

2.  Create a VAT Business Posting Group.

    1.  In the **VAT Business Posting Groups** page, select **New**.

    2.  In the **Code** field, enter EU.

    3.  In the **Description** field, enter ‘EU’.

3.  Complete the Tax Posting Setup.

    1.  In the **Tax Posting Setup** page, select **New**.

    2.  In the new tax posting setup card, fill in the following fields:

        1.  In the **VAT Bus. Posting Group** field, enter EU.

        2.  In the **VAT Prod. Posting Group** field, enter G15.

        3.  In the **VAT Calculation Type** field, enter Normal Tax.

        4.  In the **Description** field, enter ‘web shop sales’.

        5.  In the **Tax%** field, enter 15.

        6.  In the **Tax Identifier** field, enter G15.

        7.  In the **Sales Tax Account** field, enter 61850.

        8.  In the **Purchase Tax Account** field, enter 61850.

        9.  Click **Yes** to update existing records.

4.  Create a Product Posting Group.

    1.  In the **General Product Posting Groups** page, select **New**.

    2.  In the **Code** field, enter COMPUTERHW.

    3.  In the **Description** field, enter ‘computer hardware’.

    4.  In the **Def. VAT Prod. Posting Group** field, enter G15.

5.  Create a Business Posting Group

    1.  In the **Gen. Business Posting Groups** page, select **New**.

    2.  In the **Code** field, enter EU.

    3.  In the **Description** field, enter ‘EU customers and vendors’.

    4.  In the **Def. VAT Bus. Posting Group** field, enter EU.

    5.  Click **Yes** to update existing records.

    6.  In the **Gen. Business Posting Groups** page, select **New**.

    7.  In the **Code** field, enter EXPORT.

    8.  In the **Description** field, enter ‘Export customer and vendors’.

    9.  Leave the **Def. VAT Bus. Posting Group** field blank.

6.  Complete the General Posting Setup.

    1.  In the **General Posting Setup** page, select **New**.

    2.  In the new general posting setup card, in the **General** FastTab, fill
        in the following fields:

        1.  In the **Gen. Bus. Posting Group** field, fill in EU.

        2.  In the **Gen. Prod. Posting Group** field, fill in COMPUTERHW.

    3.  Select **Copy**.

    4.  In the page that opens, fill in the following fields:

        1.  In the **Gen. Bus. Posting Group** field, fill in DOMESTIC.

        2.  In the **Gen. Prod. Posting Group** field, fill in RETAIL.

        3.  In the **Copy** field, select the **All fields** option.

        4.  Leave all the checkboxes selected.

        5.  Click **OK**.

        6.  Click **Yes**.

    5.  In the new general posting setup card, in the **Sales** FastTab, change
        the following fields:

        1.  In the **Sales Account** field, change 40200 to 40210

        2.  In the **Sales Credit Memo Account** field, change 40200 to 40210

    6.  In the new general posting setup card, in the **Purchases** FastTab,
        change the following fields:

        1.  In the **Purch. Account** field, change 10700 to 50150.

        2.  In the **Purch. Credit Memo Account** field, change 10700 to 50150.

    7.  In the **General Posting Setup** page, select **New**.

    8.  In the new general posting setup card, in the **General** FastTab, fill
        in the following fields:

        1.  In the **Gen. Bus. Posting Group** field, fill in EXPORT.

        2.  In the **Gen. Prod. Posting Group** field, fill in COMPUTERHW.

    9.  Select **Copy**.

    10. In the page that opens, fill in the following fields:

        1.  In the **Gen. Bus. Posting Group** field, fill in EU.

        2.  In the **Gen. Prod. Posting Group** field, fill in COMPUTERHW.

        3.  In the **Copy** field, select the **All fields** option.

        4.  Leave all the checkboxes selected.

        5.  Click **OK**.

        6. Click **Yes**.
