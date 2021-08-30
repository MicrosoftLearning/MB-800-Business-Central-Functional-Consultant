
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

3.  Configure the new company.

### Steps

#### Task 1

Create a new company.

1. In the Get Started section on the screen, click **Start**.

3.  On the **Company Details** checklist section, click **Setup**.

3.  The **Create New Company** wizard opens.

   3.  Click **Next**.

   4.  As the company name, enter Contoso ‘*student name*’ Inc. (Replace
        ‘*student name’* with your name so that each student has its own company
        within the training database.)
    
   5. Fill in the company’s address information.

   6.  Click **Next**.
   
   9.  Specify the company’s contact details.

   10. Click **Next**.

 13. Skip the company’s bank information by clicking **Next**.
  
     
   8.  Click **Finish**.

   7.  Skip the **Fetch users from Microsoft 365** option by clicking **Skip for now**.
   
   9.  Skip the **Give permissions to users** option by clicking **Skip for now**.
    
   11.   Skip the **Manage user settings** option by clicking **Skip for now**.
    
   13.   Skip the **Set up outgoing email** option by clicking **Skip for now**.
     
   15.  Skip the **Migrate business data** option by clicking **Skip for now**.
    
   17.   Skip the **Find training on Microsoft Learn** option by clicking **Skip for now**.
  .  
   19.  Click the **Got it** button


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

3.  Create additional reporting currencies.

### Steps

### Task 1 

Complete the configuration worksheet.

   1.  From the main Business Central page in the black bar at the top of the page to the right, click the search icon,, enter 'Configuration Worksheet', and then choose the related link.
      3.  Open the **Configuration Worksheet** page.
   2.  At the bottom of the worksheet, enter a new line.
   3.  In the **Line Type** field, select **Group**.
   4.  In the **Name** field, enter ‘General Setup’.
   5.  Enter a new line.
   6.  In the **Line Type** field, select **Table**.
   7.  Open the assist edit button to the right of the **Table ID** field.
   8.  Search for ‘ZIP Code’, select table 225 and click **OK** to enter the ID
        in the **Table ID** field.
   9.  Repeat steps e. to h. to enter table 10 Shipment Method.

### Task 2

Copy data from another database company.

   1.  In the menu on the **Configuration Worksheet** page, select **More options**, then **Actions**,
        then **Tools** and then **Copy Data from Company**.

   2.  Open the assist edit button to the right of the **Copy from** field.

   3.  Select ‘Cronus USA Inc.’ and click **OK** to enter the company in the
        **Copy from** field.

   4.  Select the lines with the tables for ZIP codes and shipment methods.

   5.  In the menu select **Copy Data**.

6. In the popup, click **Yes** to confirm to copy the data.

8. Click **OK** to confirm that the data has been copied successfully


### Task 3

1. Create additional reporting currency for Denmark.

   1.  From the main Business Central page in the black bar at the top of the page to the right, click the search icon,, enter 'Currencies', and then choose the related link. Open the **Currencies** page.
   2.  In the menu on the **Currencies** page, select **+ New**.
   3.  In the **Code** field, enter **DKK**.
   4.  In the **Description** field, enter **Denmark**.
   5.  In the **ISO Code** field, enter **DKK**.
   6.  In the **ISO Numberic Code** field, enter **208**.
   7.  In the **Realized Gains Acc.** field, enter **40500**.
   8.  Close the page by clicking the left arrow button in the menu bar.

2. Create additional reporting currency for Malaysia.

    1.  Click the **+ New** button at the top of the page to enter a new record.
    3.  In the **Code** field, enter **MYR**.
    4.  In the **Description** field, enter **Malaysia**.
    5.  In the **ISO Code** field, enter **MYR**.
    6.  In the **ISO Numberic Code** field, enter **458**.
    7.  In the **Symbol** field, enter **RM**.
    8.  In the **Realized Gains Acc.** field, enter **40500**.
    9.  Close the page by clicking the left arrow button in the menu bar.

 
3. Create additional reporting currency for the UK.

   1.  Click the **+ New** button at the top of the page to enter a new record.
   3.  In the **Code** field, enter **GBP**.
   4.  In the **Description** field, enter **United Kingdom**.
   5.  In the **ISO Code** field, enter **GBP**.
   6.  In the **ISO Numberic Code** field, enter **826**.
   7.  In the **Realized Gains Acc.** field, enter **40500**.
   8.  Close the page by clicking the left arrow button in the menu bar.


4. Create additional reporting currency for South Africa.

   1.  Click the **+ New** button at the top of the page to enter a new record.
   3.  In the **Code** field, enter **ZAR**.
   4.  In the **Description** field, enter **South Africa**.
   5.  In the **ISO Code** field, enter **ZAR**.
   6.  In the **ISO Numberic Code** field, enter **710**.
   7.  In the **Symbol** field, enter **R**
   8.  In the **Realized Gains Acc.** field, enter **40500**.
   9.  Close the page by clicking the left arrow button in the menu bar.


