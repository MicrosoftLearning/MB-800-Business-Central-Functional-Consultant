---
lab:
    title: 'Lab: Set up Cash Management'
    module: 'Module 3: Configure Financials'
---

## Exercise 1: Create a bank account

### Scenario

Contoso has opened a European bank account to process customer payments of their
web shop computer hardware sales. These payments will be recorded in euro’s.
They would also like to pay their European vendors through this bank account
using the SEPA Credit Transfer format.

Details of this bank account are:

IBAN: BE13 3200 0461 4139 – BIC: BBRUBEBB

### **Tasks**

1.  Create a bank account.

2.  Assign a payment export format.

### Steps

1.  Create a bank account.

2.  At the top of the main Business Center page, click the search icon in the black bar on the right. Then type **Bank Accounts** and click the **Bank Accounts** link. 

3.  In the **Bank Accounts** page, select **New**.

4.  In the new bank accounts card, fill in the following fields:

       1.  On the **General** FastTab:

       2.  In the **No.** field, enter ‘EUROP’.

       3.  In the **Name** filed, enter ‘European bank’

       4.  On the **Posting** FastTab, in the **Currency Code** field, enter EUR. 

       5.  On the **Transfer** FastTab:

       6.  In the **SWIFT Code** field, enter BBRUBEBB

       7.  In the **IBAN** field, enter BE13 3200 0461 4139

5.  Assign a payment export format.

6.  On the **Transfer** FastTab, in the **Payment Export Format** field, enter **SEPACT**.

## Exercise 2: Set up and assign a Bank Account Posting Group

### Scenario

All transactions on the European bank account have to be posted on the balance
account 10250.

*(This general ledger account was already created in a previous lab 3.2 –
exercise 1. If not, complete this first.)*

You need to complete the correct bank posting group setup.

### Tasks

1.  Create a bank account posting group.

2.  Assign the bank account posting group.

### Steps

1.  Create a bank account posting group.

2.  In the **Bank Accounts Posting Groups** page, select **New**.

3.  In the **Code** field, enter EUROP.

4.  In the **G/L Account No.** field, enter 10250.
   
5.  Assign the bank account posting group.

6.  In the **Bank Accounts** page, open the bank account card for the
    European bank.

7.  On the **Posting** FastTab, in the **Bank Acc. Posting Group** field,
    enter the new bank account posting group ‘EUROP’.
