---
lab:
    title: 'Lab 2: Migrate master data to a new company'
    module: 'Learning Path 1: Set up Business Central'
---

Exercise 2 - Migrate master data to a new company
=================================================

Task 1: Create and export a configuration package
-------------------------------------------------

### Scenario

After completing the basic configuration, you can now start by uploading the
company's business data, such as customers, vendors, items and the chart of
accounts.

In order to prepare the migration of this data, you will configure some
configuration packages and provide these excel-files to Contoso’s super users,
to complete the information.

You will start with the vendor list, including contact information. To make sure
the users know how to complete the required information, you prepare the
following example.

The following information is returned to you by Contoso’s super user:

You will perform -

1.  Create a configuration package.

2.  Assign tables and select fields.

3.  Export a configuration package to Excel.

4.  Prepare data in Excel.

###  ***To fix the errors that occur during the lab, look at the end of the lab for fixes.***

### Steps

1.  Create a configuration package.

    1.  Select the Search icon in the top-right corner of the page,
        enter `Configuration Packages` and then choose the related link.

    2.  In the **Configuration Packages** page, select **+ New** to create a new
        configuration package.

    3.  In the **Code** field, enter `VENDOR`.

    4.  In the **Package Name** field, enter `Vendor List`.

2.  Assign tables and select fields.

    1.  On the **Tables** section of the Config. Package Card, enter a new line
        as follows.

    2.  Open the assist edit button to the right of the **Table ID** field.

    3.  In the window that opens, select the **Vendor** table and select **OK**.

    4.  Then press ENTER or TAB.

    5.  Make sure the vendor table line is selected, select **Table** and then
        **Fields**.

    6.  You will be asked to check related tables, select **No**.

    7.  Select **fields** again. On the field list page, first select **Clear
        Included**, to deselect the **Include Field** checkbox for all the
        fields.

    8.  Then select the **Include Field** checkbox for the following fields:

        1.  Name

        2.  Address

        3.  City

        4.  Phone No.

        5.  Currency Code

        6.  Language Code

        7.  Country/Region Code

        8.  Post Code

    9.  The **Validate Field** checkbox is automatically selected.

    10. Select **Close**.

3.  Export a configuration package to Excel.

    1.  In the **Config. Package Card** page, select **Export to Excel**.

    2.  Select **Yes** to export the configuration package.

4.  Prepare data in Excel.
   
    1.  Open the exported excel file from the **Downloads** folder.

    2.  Navigate to the **Vendors Import.xlsx** file (C:\ drive). Copy and paste the information as
        provided by Contoso.

    3.  Save the Excel file.

Task 2: Import and apply a configuration package
------------------------------------------------

### Scenario

When the vendor information is completed, you can now upload the vendor
information.

During this process, you want to make sure the data is validated and when
missing, the related tables will be automatically updated with newly provided
values.

You will perform -

1.  Import a configuration package from excel.

2.  Apply a configuration package.

3.  Resolve package errors.

### Steps

1.  Import a configuration package from excel.

    1.  In the **Configuration Packages** page, select the new configuration
        package for vendors and select **Manage** and then **Edit**.

    2.  In the **Config. Package Card** page, select **Import from Excel**.

    3.  Select on **Select here to browse…** and select the excel file that you
        updated in previous exercise.

    4.  Select **Open**.

    5.  Select **Import**.

2.  Apply a configuration package.

    1.  In the **Config. Package Card** page, select **Apply Package**.

    2.  Select **Yes** to confirm.

    3.  Select **OK**.

**NOTE: When you copy the Vendor records, you may be missing the Currency record for GBP. Fix this by adding the GBP record on the Currencies card.**

3.  Resolve package errors.


    1.  In the **Config. Package Card** page, the vendor table line will show a
        number of errors.

    2.  Select on the number in the **No. of Package Errors** field.

    3.  In the error page, select the first record line and select **Show
        Error**.

    4.  Select **Close**.

    5.  Repeat for all the error records.

    6.  Select **OK**.

    7.  In the **Config. Package Card** page, select the vendor table line and
        select **Table** and then select **Fields**.

    8.  Select the **Create Missing Codes** check box, for the following fields:

        1.  Currency Code

        2.  Post Code

    9.  Select **Close**.

    10. In the **Config. Package Card** page, select **Apply Package**.

    11. Select **Yes** to confirm.

    12. Select **OK**.

Task 3: Import and apply data from an existing company
---------------------------------------------

### Scenario

For the further ease of the labs during the course, you will migrate the data
from the default CRONUS USA company within the database.

You will perform -

1.  Import and apply a predefined Excel package.

### Steps

1.  Import and apply a predefined package.

    1.  In the **Configuration Packages** page, select the dropdown next to
        **Import Package**, and then select **Import from Excel**.

    2.  In the **Import From Excel** dialogue, select **select here to browse**.
    
    3.  Select the file **MB800_Lab_2.3_EVALUATION.xlsx**, and then select **Open**.

    4.  Select **Import** to confirm.
    
    **NOTE: If you get a message about dimensions, select Yes.**
    
    5.  Select on **EVALUATION**.
    
    6.  Select **Apply Package**.
    
    **NOTE: If you get a message related to duplicated contacts, select No to each message.**

    7.  Select **Yes** to continue.  

    8.  Select **Yes** to any further questions.

    9. Select **OK**.

**NOTE: You may run into errors when loading the package. You will need to fix those errors prior to continuing the labs.**

**Fixes for Errors**

You need to fix the following items:

1. Add the missing bin types from the Evaluation.xlsx file.
2. Fix/Add bin types to the White location errors
3. Increase the value for the **Contacts** number series to from 20 to 30.
4. Add three companies to **Customers**:

- School of Fine Art
- Adatum Corporation
- Trey Research

