---
lab:
    title: 'Lab 1: Create and configure a new company'
    module: 'Learning Path 1: Set up Business Central'
---

Hands-on-Lab 1: Create and configure a new company
====================================================

Exercise 1: Create a new company
--------------------------------

### Scenario

You are a functional consultant assigned to a new project, where you are
responsible for the analysis of your customers business processes. Your customer
is Contoso Ltd, situated in Redmond Washington. They will start to use
Microsoft Dynamics 365 Business Central as of their new fiscal year, January 1st
2026.

You initiate the process by creating a new company within the customers
database, including some predefined setup information but without any business
data.

### Tasks

1.  Create a new company.

2.  Complete the Company Setup wizard.

### Steps

1.  Create a new company.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Companies`, and then choose the related link.

    2.  In the **Companies** page, select the arrow by **New** and then **Create New
        Company**

    3.  The **Create New Company** wizard opens.

    4.  Select **Next**.

    5.  As the company name, enter **Contoso Ltd**.

    6.  Select the option **Production – Setup Data Only**.

    7.  Select **Next**.
    
    8.  Select **Next** on the "Available Modules" page.

    8.  Skip the **Manage Users** option by selecting **Next**.

    9.  Select **Finish** to create the company.

    10. Wait approximately 10 minutes for the company creation to complete.

    11. Refresh the **Companies** page to check the **Setup status**.

2.  Complete the **Company Setup** wizard.

    1.  Once the **Setup Status** is changed to **Completed**, go to the
        **Settings** icon on the top-right corner.

    2.  Select **My Settings** to open the new company.

    3.  Open the assist edit button (…) to the right of the **Company** textbox.

    4.  In the window that opens, select **Contoso Ltd** and select **OK**.

    >> If prompted with 'Set up a company' wizard, select **Next**. Accept the Terms & Conditions and select **Get Started**

   
    5.  Select **Settings** in the top-right corner, and then select
        **Company information**.

    6.  On the **Company Information** page, enter the following information on
        the **General** tab. Once completed, Select on the back arrow.

| Setting             | Value                 |
|---------------------|-----------------------|
| Name                | Contoso Ltd           |
| Address             | 1432 Hamilton Street |
| Address 2           | Westminster           |
| City                | Atlanta               |
| State               | GA                    |
| Zip Code            | 31772                 |
| Country/Region Code | US                    |
| Contact Name        | Alex Brown            |
| Phone Number        | \+14255550101         |

3.  Select the Search icon in the top-right corner of the page, enter
    `Accounting periods`, and then choose the related link.

4.  On the **Accounting Periods** page, select **Create Year**.

5.  On the **Create Fiscal Year** page, select **1/1/2026** in the **Starting
    Date** field.

6.  Select **OK**.

 Select on **Yes** if you receive a pop-up asking you to confirm.

7.  A new **Fiscal Year** will be displayed on the **Accounting Periods** page.

8.  Repeat for 2022 - 2025.

9.  Close all the pages.

Exercise 2: Configure a new company
-----------------------------------

### Scenario

Now that the company has been created, you will further complete the company
configuration, setup and business data.

You will start by copying the following data from the default CRONUS company:

-   Zip codes

-   Shipment methods

### Tasks

1.  Complete the configuration worksheet.

2.  Copy data from another database company.

### Steps

1.  Complete the configuration worksheet.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Configuration Worksheet` and then choose the related link.

    2.  At the bottom of the worksheet, enter a new line.

    3.  In the **Line Type** field, select **Group.**

    4.  In the **Name** field, enter `General Setup`.

    5.  Enter a new line.

    6.  In the **Line Type** field, select **Table**.

    7.  Open the assist edit button to the right of the **Table ID** field.

    8.  Search for **ZIP Code**, select table 225 and select **OK** to enter the
        ID in the **Table ID** field.

    9.  Repeat steps 5. to 8. to enter table **10 Shipment Method**.
    
**The two tables listed above already have data loaded into them. This will cause the Copy Company Data sheet to be blank. To complete this part of the exercise, you must go and delete all records in both tables in Contoso, Ltd. Go do this now. Once you've deleted all records, the Copy Company Data sheet will show the Zip Code and Shipping Method tables.**

2.  Copy data from another database company.

    1.  In the menu on the **Configuration Worksheet** page, select **Prepare**
        and then **Copy Data from Company**.

    2.  Open the assist edit button (…) to the right of the **Copy from** field.

    3.  Select **Cronus USA Inc.** and select **OK** to enter the company in the
        **Copy from** field.

    4.  Press the Shift Key and select the lines with the tables for ZIP codes and shipment methods.

    5.  In the menu select **Copy Data**.

    6.  Select **Yes**.

    7.  The data is now copied to the **Contoso Ltd** company. Select **OK**.

Close the configuration worksheet
