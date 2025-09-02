<!-- 
---
lab:
    title: 'Lab 4: Set up and use a purchase approval workflow'
    module: 'Learning Path 1: Set up Business Central'
---
-->


Hands-on-Lab 04: Set up and use a purchase approval workflow
===========================================

**Learning Objective:**
- Learners will be able to set up and use a purchase approval workflow in Dynamics 365 Business Central, including configuring workflows, setting up approval users and limits, and enabling notifications to streamline business processes.

**Business scenario:**
- You are working for a mid-sized company that needs to implement a purchase approval workflow in Dynamics 365 Business Central to ensure compliance with organizational policies and improve efficiency in handling purchase-related tasks. As a functional consultant or business user, you have been tasked with setting up the workflow, configuring approval users and limits, and enabling notifications to automate the approval process.

## Task 1: Set up approval users and define their roles, limits, and substitutes
**Goal:** Configure approval users, their roles, approval limits, and substitutes using the Approval User Setup page to ensure proper delegation and compliance with organizational policies.

1. Open the **Approval User Setup** page:
   - In the search bar, enter **Approval User Setup**, and select the related link.

2. Add a new approval user:
   - On the **Approval User Setup** page, create a new line.
   - Fill in the following fields:
     - **User ID**: Select the user involved in the approval process.
     - **Approver ID**: Specify the user who must approve requests made by the selected user.
     - **Purchase Amount Approval Limit**: Enter the maximum purchase amount the user can approve.
     - **Substitute**: Assign a substitute approver for cases when the primary approver is unavailable.

3. Define unlimited approval permissions (if applicable):
   - If the user can approve all purchase requests regardless of the amount, select the **Unlimited Purchase Approval** checkbox. Leave the **Purchase Amount Approval Limit** field blank.

4. Repeat steps 2–3 for all users who need to participate in the approval workflow.

5. Test the setup:
   - Select the **Approval User Setup Test** action to validate the configuration.

## Check your work: Set up approval users
To verify the setup:
1. Ensure all required users are listed on the **Approval User Setup** page.
2. Confirm that each user has an approver and, if necessary, a substitute assigned.
3. Validate that approval limits align with organizational policies.

---

## Task 2: Create a purchase approval workflow
**Goal:** Create a purchase approval workflow manually or from a template, defining events, conditions, and responses to automate the approval process.

1. Open the **Workflows** page:
   - In the search bar, enter **Workflows**, and select the related link.

2. Create a new workflow:
   - Select the **New** action to open the **Workflow** page.
   - In the **Code** field, enter a unique identifier for the workflow (e.g., `PURCH-APPROVAL`).
   - In the **Description** field, provide a brief description (e.g., "Purchase Approval Workflow").

3. Define the workflow steps:
   - In the **When Event** field, specify the event that triggers the workflow (e.g., "A purchase order is created").
   - In the **On Condition** field, add any conditions that must be met (e.g., "Total Amount > $10,000").
   - In the **Then Response** field, define the response (e.g., "Create an approval request for the record").

4. Add additional steps as needed:
   - For example, include steps for handling approvals, rejections, or delegations.

5. Enable the workflow:
   - Turn on the **Enabled** toggle to activate the workflow.

## Check your work: Create a purchase approval workflow
To confirm the workflow is set up correctly:
1. Review the workflow steps to ensure they align with the desired approval process.
2. Verify that the workflow is enabled and ready to trigger upon the specified event.

---

## Task 3: Configure notification settings
**Goal:** Set up notification settings to ensure relevant users are informed about pending approval requests.

1. Open the **Notification Setup** page:
   - In the search bar, enter **Notification Setup**, and select the related link.

2. Configure notification preferences:
   - Specify how users receive notifications (e.g., email or in-app).
   - Define the notification triggers (e.g., "Approval request created" or "Approval request overdue").

3. Test the notification setup:
   - Send a test notification to ensure users receive alerts as expected.

## Check your work: Configure notification settings
To validate the notification setup:
1. Confirm that notifications are sent to the correct users.
2. Verify that the notification format and content meet organizational requirements.

---

## Task 4: Test the purchase approval workflow
**Goal:** Test the workflow to ensure it functions as intended and complies with organizational policies.

1. Create a test purchase order:
   - Navigate to the **Purchase Orders** page and create a new purchase order.
   - Ensure the order meets the conditions defined in the workflow (e.g., total amount exceeds the approval threshold).

2. Trigger the workflow:
   - Submit the purchase order to initiate the approval process.

3. Verify the workflow steps:
   - Check that the approval request is sent to the designated approver.
   - Confirm that notifications are sent to the appropriate users.

4. Approve or reject the request:
   - Log in as the approver and take action on the request (approve or reject).

5. Review the outcome:
   - Ensure the workflow behaves as expected based on the approver's action.

## Check your work: Test the purchase approval workflow
To confirm the workflow is functioning correctly:
1. Verify that the approval request is routed to the correct approver.
2. Ensure notifications are sent at each step of the workflow.
3. Confirm that the purchase order status updates appropriately based on the approver's action.
