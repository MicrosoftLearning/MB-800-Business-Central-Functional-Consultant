
---
lab:
    title: 'Lab: Set up Cash Management'
    module: 'Module 3: Configure Financials'
---

Hands-on-Lab 3.7: Set Up Cash Management
========================================

Exercise 1: Create a bank account
---------------------------------

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

    1.  In the **Bank Accounts** page, select **New**.

    2.  In the new bank account card, fill in the following fields:

        1.  On the **General** FastTab:

            1.  In the **No.** field, enter ‘EUROP’.

            2.  In the **Name** filed, enter ‘European bank’

        2.  On the **Posting** FastTab, in the **Currency Code** field, enter
            **EUR**.

        3.  On the **Transfer** FastTab:

            1.  In the **SWIFT Code** field, enter BBRUBEBB

            2.  In the **IBAN** field, enter BE13 3200 0461 4139

2.  Assign a payment export format.

    1.  On the **Transfer** FastTab, in the **Payment Export Format** field,
        enter **SEPACT**.

    2.  On the **General** FastTab, in the **Credit Transfer Msg. Nos.** field,
        enter ‘CT-MSG’.

Exercise 2: Set up and assign a Bank Account Posting Group
----------------------------------------------------------

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

    1.  In the **Bank Accounts Posting Groups** page, select **New**.

    2.  In the **Code** field, enter EUROP.

    3.  In the **G/L Account No.** field, enter 10250.

2.  Assign the bank account posting group.

    1.  In the **Bank Accounts** page, open the bank account card for the
        European bank.

    2.  On the **Posting** FastTab, in the **Bank Acc. Posting Group** field,
        enter the new bank account posting group ‘EUROP’.
