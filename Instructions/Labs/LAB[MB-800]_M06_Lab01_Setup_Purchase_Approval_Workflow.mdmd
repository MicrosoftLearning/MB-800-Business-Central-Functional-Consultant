---
lab:
    title: 'Lab: Setting up and using a purchase approval workflow'
    module: 'Module 5: Integration and Automation'
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
    the purchasing agent, cannot be approved until multiple users, setup in a
    hierarchy, have approved the order.

    -   The purchasing agent can autonomously process orders up to \$5,000.00.
        All purchase orders up to \$10,000.00 are reviewed and approved by the
        purchasing manager. For all purchase orders for a higher amount the
        approval of the accounting manager is required.

    -   The accounting manager has unlimited purchase approval and manages the
        approval workflow by unblocking approval workflows.

-   Other purchase orders that are processed by the always need to be approved
    by the accounting manager alone, regardless of the amount.

-   All approvers receive an internal request note. Notes are immediately
    created at the moment of approval request.

### Tasks

1.  Setting up approval users.

2.  Setting up notifications.

3.  Creating the approval workflow.

### Steps

1.  Setting up approval users.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Approval User Setup**, and then choose the related link.

    2.  On the **Approval User Setup** page, select **+ New**.

    3.  Fill in the following fields for user 1 (accounting manager):

        1.  In the **User ID** field, enter your own user ID.

        2.  Leave the **Approver ID** field blank.

        3.  Select the **Unlimited Purchase Approval** checkbox.

        4.  Leave the **Substitute** field bank.

        5.  In the **E-mail** field, enter the e-mail for the accounting
            manager.

        6.  Select the **Approval Administrator** checkbox.

    4.  Add new users to Microsoft admin center.

        1.  Open a new tab on your browser and browse to **Microsoft admin
            center** using the given link <https://admin.microsoft.com/>.

        2.  Sign in with your **Office 365 Admin Tenant** credentials.

        3.  Select **Users \> Active users** from the left navigation pane. On
            the **Active users** page, select **Add a user**.

        4.  On the **Set up basics** page, add the following details.

            1.  **First name** – Mark

            2.  **Last name** – Brown

            3.  **Display name** – Mark Brown

            4.  **Username** – markbrown

            5.  Click **Next**.

        5.  On the **Assign product licenses** page, select **Dynamics 365
            Business Central for IWs** license, and then select **Next**.

        6.  Click **Next** on the **Optional settings** page.

        7.  On the **Review and finish** page, click **Finish adding**.

        8.  Click **Close**.

        9.  Similarly add another user with the following details.

            1.  **First name** – Sara

            2.  **Last name** – Wright

            3.  **Display name** – Sara Wright

            4.  **Username** – sarawright

    5.  Add users to Business Central

        1.  On the Users page, select update users from Microsoft 365

        2.  Click **Next**.

        3.  Click **Finish**.

        4.  Click **Close**.

        5.  The newly created users are added to Business Central.

    6.  On the **Approval User Setup** page, select **+ New**.

    7.  Fill in the following fields for user 2 (purchasing manager):

        1.  In the **User ID** field, enter **Mark Brown**.

        2.  In the **Approver ID** field, enter the accounting manager ID,
            **ADMIN**.

        3.  In the **Purchase Amount Approval Limit** field, enter
            **10,000.00**.

        4.  Leave the **Substitute** field bank.

        5.  In the **E-mail** field, enter the e-mail
            **markbrown\@M365x09767429.onmicrsoft.com**.

        6.  Leave the **Approval Administrator** checkbox unselected.

    8.  On the **Approval User Setup** page, select **+ New**.

    9.  Fill in the following fields for user 3 (purchasing agent):

        1.  In the **User ID** field, enter **Sara Wright**.

        2.  In the **Approver ID** field, enter the purchasing manager ID,
            **MARKBROWN**.

        3.  In the **Purchase Amount Approval Limit** field, enter **5,000.00**.

        4.  Leave the **Substitute** field bank.

        5.  In the **E-mail** field, enter the e-mail of purchasing agent
            **sarawright\@M365x09767429.onmicrsoft.com**.

        6.  Leave the **Approval Administrator** checkbox unselected.

2.  Setting up notifications.

    1.  From the **Approval User Setup** page, select the line for user 1.

    2.  Select **Notification Setup**.

    3.  On the opened **Notification Setup** page, select **+ New**.

        1.  In the **Notification Type** field, enter **Approval.**

        2.  In the **Notification Method** field, enter **Note**.

        3.  Select **Notification Schedule**

            1.  In the **Recurrence** field, enter **Instantly**.

            2.  Close the **Notification Schedule** page.

        4.  Close the **Notification Setup Page**.

    4.  Repeat steps a to c for users 2 and 3.

3.  Creating the approval workflow.

    1.  Select the search for page icon in the top-right corner of the page,
        enter **Workflow Templates**, and then choose the related link.

    2.  On the **Workflow Templates** page, select **Purchase Order Approval
        Workflow**.

    3.  Select **New** and then select **New Workflow from Template**.

    4.  A workflow is created, in the **Code** field, the value **MS-POAPW-01**
        is automatically filled in.

    5.  On the **Worflow Steps** FastTab, select the first line where the **When
        Event** field contains the value **Approval of a purchase document is
        requested**

    6.  Click on the **On Condition** field.

        1.  Select the **Document Type** filter and enter **Order**.

        2.  Select the **Status** filter and enter **Open**.

        3.  Click **+ Filter**

        4.  Select the **Gen. Bus. Posting Group** filter and enter **EU**.

        5.  Click **OK** to close the **Event Conditions** page.

    7.  Click on the **Then Response** field.

        1.  Select response **Create an approval request for the record using
            type Approver and approver limit type Approver Chain**.

            1.  On the **Options for the Selected Response** FastTab, make sure
                the following fields are filled in:

                1.  In the **Approver Type** field, enter **Approver**.

                2.  In the **Approver Limit Type** field, enter **Approver
                    Chain**.

        2.  Click **OK** to close the **Workflow Responses** page.

    8.  Select the **Enabled** checkbox.

    9.  Close the workflow.

    10. On the **Workflow Templates** page, select **Purchase Order Approval
        Workflow**.

    11. Select **New** and then select **New Workflow from Template**.

    12. A workflow is created, in the **Code** field, the value **MS-POAPW-02**
        is automatically filled in.

    13. On the **Worflow Steps** FastTab, select the first line where the **When
        Event** field contains the value **Approval of a purchase document is
        requested**

    14. Click on the **On Condition** field.

        1.  Select the **Document Type** filter and enter **Quote**.

        2.  Select the **Status** filter and enter **Open**.

        3.  Select the **Gen. Bus. Posting Group** filter and enter **EU**.

        4.  Click **OK** to close the **Event Conditions** page.

    15. Click on the **Then Response** field.

        1.  Select response **Create an approval request for the record using
            type Approver and approver limit type Approver Chain**.

            1.  On the **Options for the Selected Response** FastTab, change the
                following fields are filled in:

                3.  In the **Approver Type** field, enter **Approver**.

                4.  In the **Approver Limit Type** field, enter **Specific
                    Approver**.

                5.  In the **Approver ID** field, enter your own ID, for the
                    accounting manager.

        2.  Click **OK** to close the **Workflow Responses** page.

    16. Select the **Enabled** checkbox.

    17. Close the workflow.

Exercise 2: Using a purchase approval workflow
----------------------------------------------

### Scenario

The purchasing agent places an order with vendor School of Fine Art on January
14th, 2023, for the following items:

-   45 pieces quitkey keyboards at \$50.00 a piece

-   75 pieces speakers at \$38.00 a piece

### Tasks

1.  Request approval of a purchase order.

2.  Receiving a notification and approving the request.

### Steps

1.  Request approval of a purchase order.

    1.  Log in the database as the purchasing agent.

        1.  Sign in to Microsoft 365 admin center <https://admin.microsoft.com>
            with your Office 365 admin tenant credentials.

        2.  Select **Users \> Active users** from the left navigation pane. On
            the **Active users** page, and then select the user **Sara Wright**.

        3.  Click **Reset password**.

        4.  Select the checkbox against **Automatically create a password** and
            click **Reset password**.

        5.  **Copy** the username and password and save it in a **Notepad**.

        6.  Sign in to Business Central with the username
            <sarawright@M365x09767429.onmicrosoft.com> and the given password

    2.  Select the search for page icon in the top-right corner of the page,
        enter **Purchase Orders**, and then choose the related link.

    3.  On the **Purchase Orders** page, select **+ New**.

    4.  On the opened purchase order, on the **General** FastTab, click **Show
        more** and then fill in the following fields.

        1.  In the **Vendor No.** field, enter **V9005**.

        2.  In the **Posting Date** and **Order Date** fields, enter
            **1/14/2023**.

    5.  On the **Lines** section, create a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1005** for the **Quietkey
            keyboards**.

        3.  In the **Location Code** field, enter **MAIN**.

        4.  In the **Quantity** field, enter **45**.

        5.  In the **Direct Unit Cost Excl. Tax** field, enter **50.00**.

        6.  In the **Tax Group Code**, enter **NONTAXABLE**.

    6.  On the **Lines** section, create a new line by filling in the following
        fields:

        1.  In the **Type** field, enter **Item**.

        2.  In the **No.** field, enter **CHW1006** for the speakers.

        3.  In the **Location Code** field, enter **MAIN**.

        4.  In the **Quantity** field, enter **75**.

        5.  In the **Direct Unit Cost Excl. Tax** field, enter **38.00**.

        6.  In the **Tax Group Code**, enter **NONTAXABLE**.

    7.  Select **Request Approval** and then select **Send Approval Request**.

    8.  Click **OK**.

    9.  In the **Status** field, the value is automatically set to **Pending
        Approval**.

    10. Select the search for page icon in the top-right corner of the page,
        enter **Sent Notification Entries**, and then choose the related link.

    11. On the **Sent Notification Entries** page, a new entry is created.

2.  Receiving a notification and approving the request.

    1.  Log in the database as the purchasing manager.

        1.  Navigate back to **Microsoft 365 admin center**

        2.  Select **Users \> Active users** from the left navigation pane. On
            the **Active users** page, and then select the user **Mark Brown**.

        3.  Click **Reset password**.

        4.  Select the checkbox against **Automatically create a password** and
            click **Reset password**.

        5.  **Copy** the username and password and save it in a **Notepad**.

        6.  Sign in to Business Central with the username
            <markbrown@M365x09767429.onmicrosoft.com> and the given password

    2.  Select the search for page icon in the top-right corner of the page,
        enter **Requests to Approve**, and then choose the related link.

    3.  On the **Requests to Approve** page, select the line for the purchase
        order.

    4.  Select **Approve**.

    5.  Log in to Business Central with purchase agent’s credentials **Sara
        Wright**.

    6.  Select the search for page icon in the top-right corner of the page,
        enter **Purchase orders**, and then choose the related link.

    7.  On the purchase order, the **Status** field is changed to **Released**.
