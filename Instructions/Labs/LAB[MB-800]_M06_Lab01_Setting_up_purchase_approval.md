
---
lab:
    title: 'Lab: Setting up and using a purchase approval workflow'
    module: 'Module 6: Integration and Automation'
---

Hands-on-Lab 6.1: Setting up and using a purchase approval workflow
===================================================================

Exercise 1: Setting up a purchase approval workflow
---------------------------------------------------

### Scenario

*Remark: You must make sure that at least three users exist in Business
Central.*

-   *User 1 = Accounting manager (take your own account for this role)*

-   *User 2 = Purchase manager (take the account from one of the fellow students
    for this role)*

-   *User 3 = Purchasing agent (take the account from one of the fellow students
    for this role)*

Contoso would like to start using an approval workflow for purchase orders
processed by the purchasing agent. Hereby the following requirements need to be
met:

-   The purchase orders, placed with a vendor located in Europe and processed by
    the purchasing agent, cannot be approved until multiple users, setup in an
    hierarchy, have approved the order.

    -   The purchasing agent is allowed to autonomously process orders up to LCY
        5,000.00. All purchase orders up to LCY 10,000.00 are reviewed and
        approved by the purchasing manager. For all purchase orders for a higher
        amount the approval of the accounting manager is required.

    -   The accounting manager has unlimited purchase approval and also manages
        the approval workflow by unblocking approval workflows.

-   Other purchase orders that are processed by the purchasing agent always need
    to be approved by the accounting manager alone, regardless of the amount.

-   All approvers receive an internal request note. Notes are immediately
    created at the moment of approval request.

### Tasks

1.  Setting up approval users.

2.  Setting up notifications.

3.  Creating the approval workflow.

### Steps

1.  Setting up approval users.

    1.  On the **Approval User Setup** page, select **New**.

    2.  Fill in the following fields for user 1 (accounting manager):

        1.  In the **User ID** field, enter your own user ID.

        2.  Leave the **Approver ID** field blank.

        3.  Select the **Unlimited Purchase Approval** checkbox.

        4.  Leave the **Substitute** field bank.

        5.  In the **E-mail** field, enter the e-mail for the accounting
            manager.

        6.  Select the **Approval Administrator** checkbox.

    3.  On the **Approval User Setup** page, select **New**.

    4.  Fill in the following fields for user 2 (purchasing manager):

        1.  In the **User ID** field, enter a user ID.

        2.  In the **Approver ID** field, enter the accounting manager ID.

        3.  In the **Purchase Amount Approval Limit** field, enter 10,000.00.

        4.  Leave the **Substitute** field bank.

        5.  In the **E-mail** field, enter the e-mail for the purchasing
            manager.

        6.  Leave the **Approval Administrator** checkbox unselected.

    5.  On the **Approval User Setup** page, select **New**.

    6.  Fill in the following fields for user 3 (purchasing agent):

        1.  In the **User ID** field, enter a user ID.

        2.  In the **Approver ID** field, enter the purchasing manager ID.

        3.  In the **Purchase Amount Approval Limit** field, enter 5,000.00.

        4.  Leave the **Substitute** field bank.

        5.  In the **E-mail** field, enter the e-mail for the purchasing agent.

        6.  Leave the **Approval Administrator** checkbox unselected.

2.  Setting up notifications.

    1.  From the **User Approval Setup** page, select the line for user 1.

    2.  Select **Notification Setup**.

    3.  On the opened **Notification Setup** page, select **New**.

        1.  In the **Notification Type** field, enter **Approval.**

        2.  In the **Notification Method** field, enter **Note**.

        3.  Select **Notification Schedule**

            1.  In the **Recurrence** field, enter **Instantly**.

            2.  Close the **Notification Schedule** page.

        4.  Close the **Notification Setup Page**.

    4.  Repeat steps a to c for users 2 and 3.

3.  Creating the approval workflow.

    1.  On the **Workflow Templates** page, select **Purchase Order Approval
        Workflow**.

    2.  Select **Actions** and then select **New Workflow from Template**.

    3.  A workflow is created, in the **Code** field, the value MS-POAPW-01 is
        automatically filled in.

    4.  On the **Worflow Steps** FastTab, select the first line where the **When
        Event** field contains the value ‘Approval of a purchase document is
        requested’

    5.  Click on the **On Condition** field.

        1.  Select the **Document Type** filter, and enter ‘Order’.

        2.  Select the **Status** filter, and enter ‘Open’.

        3.  Select the **Gen. Bus. Posting Group** filter, and enter ‘EU’.

        4.  Click **OK** to close the **Event Conditions** page.

    6.  Click on the **Then Response** field.

        1.  Select response ‘Create an approval request for the record using
            type Approver and approver limit type Approver Chain’.

            1.  On the **Options for the Selected Response** FastTab, make sure
                the following fields are filled in:

                1.  In the **Approver Type** field, enter **Approver**.

                2.  In the **Approver Limit Type** field, enter **Approver
                    Chain**.

        2.  Click **OK** to close the **Workflow Responses** page.

    7.  Select the **Enabled** checkbox.

    8.  Close the workflow.

    9.  On the **Workflow Templates** page, select **Purchase Order Approval
        Workflow**.

    10. Select **Actions** and then select **New Workflow from Template**.

    11. A workflow is created, in the **Code** field, the value MS-POAPW-02 is
        automatically filled in.

    12. On the **Worflow Steps** FastTab, select the first line where the **When
        Event** field contains the value ‘Approval of a purchase document is
        requested’

    13. Click on the **On Condition** field.

        1.  Select the **Document Type** filter, and enter ‘Order’.

        2.  Select the **Status** filter, and enter ‘Open’.

        3.  Select the **Gen. Bus. Posting Group** filter, and enter ‘EU’.

        4.  Click **OK** to close the **Event Conditions** page.

    14. Click on the **Then Response** field.

        1.  Select response ‘Create an approval request for the record using
            type Approver and approver limit type Approver Chain’.

            1.  On the **Options for the Selected Response** FastTab, change the
                following fields are filled in:

                3.  In the **Approver Type** field, enter **Approver**.

                4.  In the **Approver Limit Type** field, enter **Specific
                    Approver**.

                5.  In the **Approver ID** field, enter your own ID, for the
                    accounting manager.

        2.  Click **OK** to close the **Workflow Responses** page.

    15. Select the **Enabled** checkbox.

    16. Close the workflow.

Exercise 2: Using a purchase approval workflow
----------------------------------------------

### Scenario

The purchasing agent places an order with vendor Cronus Cardoxy Sales on January
14th, 2022, for the following items:

-   45 pieces quitkey keyboards at LCY 50.00 a piece

-   75 pieces speakers at LCY 38.00 a piece

The items are to be delivered in the European warehouse.

### Tasks

1.  Request approval of a purchase order.

2.  Receiving a notification and approving the request.

### Steps

1.  Request approval of a purchase order.

    1.  Log in the database as the purchasing agent.

    2.  On the **Purchase Orders** page, select **New**.

    3.  On the opened purchase order, on the **General** FastTab, fill in the
        following fields.

        1.  In the **Vendor No.** field, enter V9002.

        2.  In the **Posting Date** and **Order Date** fields, enter 1/14/2022.

    4.  On the **Lines** section, create a new line by filling in the following
        fields:

        1.  In the **Type** field, enter Item.

        2.  In the **No.** field, enter CHW1005 for the quietkey keyboards.

        3.  In the **Location Code** field, the value EUROP is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, the value PCS is
            automatically filled in.

        5.  In the **Quantity** field, enter 45.

        6.  In the **Direct Unit Cost Excl. Tax** field, enter 50.00.

    5.  On the **Lines** section, create a new line by filling in the following
        fields:

        1.  In the **Type** field, enter Item.

        2.  In the **No.** field, enter CHW1006 for the speakers.

        3.  In the **Location Code** field, the value EUROP is automatically
            filled in.

        4.  In the **Unit of Measure Code** field, change the value to PCS.

        5.  In the **Quantity** field, enter 75.

        6.  In the **Direct Unit Cost Excl. Tax** field, enter 38.00.

    6.  Select **Request Approval** and then select **Send Approval Request**.

    7.  Click **OK**.

    8.  In the **Status** field, the value is automatically set to **Pending
        Approval**.

    9.  On the **Sent Notification Entries** page, a new entry is created.

2.  Receiving a notification and approving the request.

    1.  Log in the database as the purchasing manager.

    2.  On the **Requests to Approve** page, select the line for the purchase
        order.

    3.  Select **Approve**.

    4.  On the purchase order, the **Status** field is changed to **Released**.
