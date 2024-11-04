Exercise 8: Set Up Cash Management
==================================

Task 1: Create a bank account
-----------------------------

### Scenario

Contoso has opened a European bank account to process customer payments of their
web shop computer hardware sales. These payments will be recorded in euros. They
would also like to pay their European vendors through this bank account using
the SEPA Credit Transfer format.

Details of this bank account are:

IBAN: BE13 3200 0461 4139 – BIC: BBRUBEBB

You will perform:

1.  Create a bank account.

2.  Assign a payment export format.

### Steps

1.  Create a bank account.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Bank Accounts` and then choose the related link.

    2.  In the **Bank Accounts** page, select **+ New**.

    3.  In the new bank accounts card, fill in the following fields:

        1.  On the **General** FastTab:

            1.  In the **No.** field, enter `EUROP`.

            2.  In the **Name** filed, enter `European bank`

        2.  On the **Posting** FastTab, in the **Currency Code** field, select
            **EUR**.

        3.  On the **Transfer** FastTab:

            1.  Click **Show more**.

            2.  In the **SWIFT Code** field, enter `BBRUBEBB`

            3.  In the **IBAN** field, enter `BE13 3200 0461 4139`

2.  Assign a payment export format.

    1.  On the **Transfer** FastTab, in the **Payment Export Format** field,
        enter `SEPACT`.

Exercise 2: Set up and assign a Bank Account Posting Group
----------------------------------------------------------

### Scenario

All transactions on the European bank account have to be posted on the balance
account 10250.

*(This general ledger account was already created in a previous lab 3.2 –
exercise 1. If not, complete this first.)*

You need to complete the correct bank posting group setup.

You will perform:

1.  Create a bank account posting group.

2.  Assign the bank account posting group.

### Steps

1.  Create a bank account posting group.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Bank Accounts Posting Group` and then choose the related link.

    2.  In the **Bank Accounts Posting Groups** page, select **+ New**.

    3.  In the **Code** field, enter `EUROP`.

    4.  In the **G/L Account No.** field, enter **10250**.

Note – If you do not find the G/L Account No. – Please proceed with creating a
new.

2.  Assign the bank account posting group.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Bank Accounts` and then choose the related link.

    2.  In the **Bank Accounts** page, open the bank account card for the
        **European bank**.

    3.  On the **Posting** FastTab, in the **Bank Acc. Posting Group** field,
        select the new bank account posting group **EUROP**.

