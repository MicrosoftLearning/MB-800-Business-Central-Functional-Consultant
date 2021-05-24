---
lab:
    title: 'Lab: Create and configure a new company'
    module: 'Module 2: Application Setup'
---

# Create and configure a new company

## Exercise 1: Create a new company

### Scenario

You are a functional consultant assigned to a new project, where you are
responsible for the analysis of your customers business processes. Your customer
is Contoso Inc., situated in Redmond Washington. They will start to use
Microsoft Dynamics 365 Business Central as of their new fiscal year, January 1st
2021.

You initiate the process by creating a new company within the customers
database, including some predefined setup information but without any business
data.

### Tasks

1.  Create a new company.

2.  Complete the Company Setup wizard.

### Steps

1.  Create a new company.

2.  In the **Companies** page, select **New** and then, **Create New
    Company**. To find the **Companies** page use the search icon located in the black bar at the top of the page on the right hand side.

3.  The **Create New Company** wizard opens.

4.  Click **Next**.

5.  As the company name, enter Contoso ‘*student name*’ Inc. (Replace
    ‘*student name’* with your name so that each student has its own company
    within the training database.)

6.  Select the option **Production – Setup Data Only**.

7.  Click **Next**.

8.  Skip the **Manage Users** option by clicking **Next**.

9.  Click **Finish** to create the company.

    **Note:** This may take 10 to 15 minutes and you will need to wait until the status shows completed.

10.  Complete the **Company Setup** wizard.

11.  To open the new company, go to the **My Settings** page.

12.  Open the assist edit button to the right of the **Company** textbox.

13.  In the window that opens, select “Contoso ‘*student name*’ Inc.” and
    click **OK**.

14.  Click **OK**.

15.  The new company opens and the **Company Setup** wizard automatically
    opens.

16.  Click **Next**.

17.  Fill in the company’s address information.

18.  Click **Next**.

19.  Specify the company’s contact details.

20. Click **Next**.

21. Disable the **Use a bank feed service** option.

22. Click **Next**.

23. Skip the company’s bank information by clicking **Next**.

24. In the **Fiscal Year Start Date** field, enter 1/1/2021.

25. Click **Next**.

26. Leave the costing method set to the default value ‘FIFO’.

27. Click **Next**.

28. Click **Finish** to start using the company.

## Exercise 2: Configure a new company

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

2.  Open the **Configuration Worksheet** page by clicking on the search icon in the black bar at the top of the page on the right hand side, then type **Configuration Worksheet**. Then select the **Configuration Worksheet** link.

3.  At the bottom of the worksheet, enter a new line.

4.  In the **Line Type** field, select **Group.**

5.  In the **Name** field, enter ‘General Setup’.

6.  Enter a new line.

7.  In the **Line Type** field, select **Table**.

8.  Open the assist edit button to the right of the **Table ID** field.

    **Note:** The assist edit button is the box to the right with the ellipsys.

9.  Search for ‘ZIP Code’, select table 225 and click **OK** to enter the ID
    in the **Table ID** field.

10.  Repeat steps e. to h. to enter table 10 Shipment Method.

11.  Copy data from another database company.

12.  In the menu on the **Configuration Worksheet** page, select **Actions**,
    then **Tools** and then **Copy Data from Company**.

13.  Open the assist edit button to the right of the **Copy from** field.

14.  Select ‘Cronus USA Inc.’ and click **OK** to enter the company in the
    **Copy from** field.

15.  Select the lines with the tables for ZIP codes and shipment methods.

16.  In the menu select **Copy Data**.

17.  The data is now copied in the new company.
