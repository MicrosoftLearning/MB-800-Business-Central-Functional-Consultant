---
lab:
    title: 'Lab: Set up General Journals'
    module: 'Module 3: Configure Financials'
---

Hands-on-Lab 3.5: Set Up General Journals
=========================================

Exercise 1: Set up General Journals
-----------------------------------

### Scenario

Part of the implementation process is the conversion of opening balances. For
these specific transactions a separate general journal OPENING will be created.

Separate batches are set up for the entry of the opening g/l balance accounts,
the open customer ledger entries, the open vendor ledger entries and the opening
bank balance.

For customers and vendors the detailed open ledger entries will be entered using
the existing document no. given by the previous system. The total amount will be
balanced by the regular g/l accounts for accounts receivables (10400) and
accounts payable (20100).

You also want to avoid any tax postings while entering the opening g/l balances.

### Tasks

1.  Set up a journal for opening entries

2.  Set up different batches for customer, vendor, balance

### Steps

1.  Set up a journal for opening entries

    1.  In the **General Journal Templates** page, select New.

    2.  Fill in the following fields:

        1. In the **Name** field, enter **OPENING**

        2. In the **Description** field, enter **conversion opening balances**.

        3.  In the **Type** field, select the **General** option.

        4.  In the **Bal. Account Type** field, select the **G/L Account**
            option.

        5.  Deselect the **Force Doc. Balance** check box.

        6.  Deselect the **Copy Tax Setup to Jnl.** check box.

        7.  Click **Yes**.

2.  Set up different batches for customer, vendor, balance and bank.

    1.  In the **General Journal Templates** page, make sure the OPENING journal
        is selected.

    2.  Select **More options**, then **Related**, then select **Template** and then select
        **Batches**.

    3.  In the opened **General Journal Batches** page, select **New**.

    4.  Fill in the following fields:

        1.  In the **Name** field, enter BALANCE.

        2.  In the **Description** field, enter ‘opening g/l balance account’.

    5.  In the opened **General Journal Batches** page, select **New**.

    6.  Fill in the following fields:

        1.  In the **Name** field, enter BANK.

        2.  In the **Description** field, enter ‘opening bank balance’.

    7.  In the opened **General Journal Batches** page, select **New**.

    8.  Fill in the following fields:

        1.  In the **Name** field, enter CUST.

        2.  In the **Description** field, enter ‘opening customer ledger
            entries’.

        3.  In the **Bal. Account No.** field, enter 10400

    9.  In the opened **General Journal Batches** page, select **New**.

    10. Fill in the following fields:

        1.  In the **Name** field, enter VEND.

        2.  In the **Description** field, enter ‘opening vendor ledger entries’.

        3.  In the **Bal. Account No.** field, enter 20100
