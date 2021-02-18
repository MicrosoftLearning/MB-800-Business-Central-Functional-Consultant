---
lab:
    title: 'Lab: Set up General Journals'
    module: 'Module 3: Configure Financials'
---

## Exercise 1: Set up General Journals

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

2.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **General Journal Templates**, and click the the **General Journal Templates** link. 

3.  In the **General Journal Templates** page, select **New**.

4.  Fill in the following fields:

       1.  In the **Name** field, enter OPENING

       2.  In the **Description** field, enter ‘conversion opening balances’.

       3.  In the **Type** field, select the **General** option.

       4.  In the **Bal. Account Type** field, select the **G/L Account**
            option.

       5.  Deselect the **Force Doc. Balance** check box.

       6.  Deselect the **Copy Tax Setup to Jnl.** check box.

5.  Set up different batches for customer, vendor, balance, and bank.

6.  In the **General Journal Templates** page, make sure the OPENING journal
    is selected.

7.  Select **Related**, then select **Template** and then select
    **Batches**.

8.  In the opened **General Journal Batches** page, select **New**.

9.  Fill in the following fields:

       1.  In the **Name** field, enter BALANCE.

       2.  In the **Description** field, enter ‘opening g/l balance account’.

10. In the opened **General Journal Batches** page, select **New**.

11. Fill in the following fields:

       1.  In the **Name** field, enter BANK.

       2.  In the **Description** field, enter ‘opening bank balance’.

12. In the opened **General Journal Batches** page, select **New**.

13. Fill in the following fields:

       1.  In the **Name** field, enter CUST.

       2.  In the **Description** field, enter ‘opening customer ledger
            entries’.

       3.  In the **Bal. Account No.** field, enter 10400

14. In the opened **General Journal Batches** page, select **New**.

15. Fill in the following fields:

       1.  In the **Name** field, enter VEND.

       2.  In the **Description** field, enter ‘opening vendor ledger entries’.

       3.  In the **Bal. Account No.** field, enter 20100
