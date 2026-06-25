---
lab:
  title: 'Lab 13: Manage accounting period'
  module: 'Close a fiscal year in Dynamics 365 Business Central'
  duration: 30 minutes
  level: 300
  islab: true
---


## Exercise 13: Manage accounting period.



## Task 1: Close posting period for the user.

## Scenario
Your task is to manage the accounting periods in Business Central by closing the posting period 2025 for selected users. You will restrict posting dates for a specific user to avoid posting entries in the closed period.


Select the Search icon in the top-right corner of the page, enter User Setup and then choose the related link.

In the User Setup page, in the new line select User ID.
In the Allow Posting from field enter 1/1/26.

Close User Setup.

## Task 2: Close posting period for everyone.

## Scenario
As part of the year
end process, you must ensure that no users can post new transactions into the period 2025 that has just closed. After reviewing the company’s accounting calendar, management has confirmed that all entries for the month are complete. To protect the integrity of financial data, your task is to close the posting period for all users so that no further postings can be made in that timeframe.


Select the Search icon in the top-right corner of the page, enter General Ledger Setup and then choose the related link.
	On the General FastTab

In the Allow Posting from field, enter 1/1/26.

Close General Ledger Setup.


## Task 3: Close fiscal year.

## Scenario
As the company completes its year
end activities, all financial transactions for the fiscal year have been reviewed, adjusted, and finalized. Management has confirmed that no additional postings should be made to the closing 2025 year. Your task is to close the fiscal year in Business Central to lock the period and prevent further changes. You will complete the year
end closing process so the system can begin the new fiscal year with accurate, protected financial data.

You will perform:

- Close Accounting period.

- Prepare and post Income Statement closing entries.


### Steps

1. Close Accounting period.

2. Select the Search icon in the top-right corner of the page, enter Accounting periods, and then choose the related link.

3. On the Accounting Periods page, select the line for 1/1/2025.

4. On the menu, select Close Year.


5. Prepare and post Income Statement closing entries.

6. Select the Search icon in the top-right corner of the page, enter Close Income Statement, and then choose the related link.
On the Close Income Statement page

7. In the Fiscal Year Ending Date field 12/31/25 is automatically populated.
In the Gen. Journal Template field, select GENERAL.
In the  Gen. Journal Batch, select +New and add new line with Name –CLOSE, Description – Close year.
Select OK.

8. In the Document No. field, enter CL2025.
In the Retained Earnings Acc. field, enter 30310 Results for the Financial year account.
In the Post to Retained Earnings Acc., select - Balance.
In the Posting Description field, enter Close Income Statement 2025.
In the Dimensions field, select DEPARTMENT and BUSINESSGROUP, select Close.

9. Select OK.
Select OK.


Select the Search icon in the top-right corner of the page, enter User Setup and then choose the related link.

In the User Setup page, in the new line select User ID.
In the Allow Posting from field, remove value.

Close User Setup.

Select the Search icon in the top-right corner of the page, enter General Ledger Setup and then choose the related link.
	On the General FastTab

In the Allow Posting from field, remove value.

Close General Ledger Setup.


10. Select the Search icon in the top-right corner of the page, enter General Journals, and then choose the related link.
On the General Journal Template list page, select GENERAL.

11. On the Batch Name field, select CLOSE value.
On the menu select Home, Post, Post.







