---
lab:
  title: 'Lab 24: Reconcile customer and vendor entries'
  module: 'Enter payments in the cash receipt journal and the payment journal in Dynamics 365 Business Central'
  duration: 30 minutes
  level: 300
  islab: true
---


## Exercise 24: Reconcile customer and vendor entries


## Task 1: Post payment entries in the journal.


## Scenario
You are the Accountant responsible for managing the company’s receivables and payables. Since the company does not have bank integration for the USD bank account and you must manually enter these payments using cash receipt journal. 
Bank account details: World Wide Bank, branch – BG99999, account - 99-44-567.
List of payments:


| Date | Counterparty | Reference | Amount, $ |
| --- | --- | --- | --- |
| 12/1/25 | Wide World Importers | WW25/367 | -1600 |
| 1/1/26 | Wide World Importers | WW25/26 | -3600 |
| 1/1/26 | Trey Research |  | 2000 |


You will perform:

- Create Bank account

- Set up Cash Receipt journal batch

- Create, reconcile and post payment entries.



### Steps
1. Create a bank account.

2. Select the Search icon in the top-right corner of the page, enter Bank Accounts and then choose the related link.

3. In the Bank Accounts page, select + New.

4. In the new bank accounts card, fill in the following fields:

5. On the General FastTab:

6. In the No. field, enter USD.

7. In the Name field, enter World Wide Bank.

8. In the Bank Branch No. field enter BG99999.

9. In the Bank Account No. field, enter 99-44-567.

10. On the Posting FastTab:

11. The Currency Code field leaves blank.

12. In the Bank Acc.Posting Group field, enter OPERATING.

13. Select No.

14. Set up Cash Receipt journal.

15. Select the Search icon in the top-right corner of the page, enter Cash Receipt journals and then choose the related link.

16. On the opened General Journal Batches page, select + New and fill in the following fields:

17. In the Name field, enter USD.

18. In the Description field, enter World Wide Bank.

19. In the Bal. Account Type field, enter Bank Account.

20. In the Bal. Account No. field, enter OPERATING.

21. In the No. Series field, the value GJNL-PMT is automatically filled in.

22. Select OK.

23. The new batch OPERATING is automatically filled in in the Batch Name field on the cash receipt journal.

24. Create payment entries.

25. In the Cash Receipt journal, fill in the details for the new line.
    Enter in the Posting Date field 12/1/25.
	Select in the Document type field, the option Payment.
	Select in the Account type field, the option Vendor.
	Select in the Account no. field 40000 for Wide World Importers vendor.
	Enter in the Amount field 1600.
	Select in the Applies-to Doc.Type field, the value Invoice.
	On the Apply Vendor Entries page select the line with invoice from 12/1/25 and External Document No. WW25/367

26. Select OK.

27. In the Cash Receipt journal, fill in the details for the new line.

28. Enter in the Posting Date field 1/1/26.

29. Select in the Document type field, the option Payment.

30. Select in the Account type field, the option Vendor.
31. Select in the Account no. field 40000 for Wide World Importers vendor.

32. Enter in the Amount field 3600.
33. On the menu select Home, Apply Entries.
34. On the Apply Vendor Entries select the lines: 
			the line with External Document No. WW25/368, Posting Date 12/10/2025
			the line with External Document No. WW26/001, Posting Date 1/1/2026
			the line with External Document No. WW26/002, Posting Date 1/10/2026
			Select Set Applies –to ID

35. The system shows the message “You cannot apply and post an entry to an entry with an earlier posting date...”, select **OK**.

36. Unselect the line with External Document No. WW26/002, Posting Date 1/10/2026.

37. Select Set Applies –to ID, to assign value for the Applies to ID field.
38. Select **OK**.
39. In the Cash Receipt journal, fill in the details for the new line.
40. Enter in the Posting Date field 1/1/26.
41. Select in the Document type field, the option Payment.
42. Select in the Account type field the option Customer.
43. Select in the Account no. field 20000 for Trey Research.
44. Enter in the Amount field -2000.
45. Select in the Applies-to Doc.Type field, the value Invoice.
46. On the Apply Customer Entries page select the line with invoice from 12/16/25
47. Select OK.
48. Select Home, and then select Post.
49. Select Yes.
50. Select OK.


## Task 2: Reconcile posted entries.

## Scenario
After recording incoming and outgoing payments, you must reconcile the related ledger entries to reflect accurate balances for vendor 40000 Wide World Importers.

You will perform:

- Reconcile posted entries.

- Review detailed vendor entries and applied entries.



### Steps
1. Reconcile posted entries.

2. Select the Search icon in the top-right corner of the page, enter Vendors and then choose the related link.

3. On the Vendor list page select line with 40000 Wide World Importers.

4. Select on the menu Vendor, Ledger Entries
	On the Vendor Ledger entries page,
	Select the red invoice line with External Document No. WW26/002.
	Select on the menu Apply Entries, Apply Entries.
	On the Apply Vendor Entries page, select Set Applies –to ID to assign value for the Applies to ID field for the line with payment entry.
	Select Post Application.

5. On the Post application page, leave the Document No. - P26/0005 and Posting Date -1/10/2026.
	Select OK.

6. Select OK.


7. Review detailed vendor entries and applied entries.

8. On the Vendor Ledger entries page

9. Select the payment dated 1/1/26 with Original Amount = 3600 and Remaining Amount = 0

10. Select on the menu of Entry, Applied Entries.
	Review the invoices closed by this payment and confirm that the Sum of Closed by Amount = 3600.

Close Applied Vendor Entries.

11. Select on the menu of Entry, Detailed Ledger Entries.

12. In Detailed Vendor Ledger Entries, verify the following:

13. A Payment Initial Entry for 3600

14. A Payment Application Entry for 2600 (applied during payment posting)

15. An Invoice Application Entry for 1000 (applied during reconciliation)













