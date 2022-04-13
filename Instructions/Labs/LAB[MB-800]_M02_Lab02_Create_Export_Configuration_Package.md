---
lab:
    title: 'Lab: Create and export a configuration package'
    module: 'Module 2: Application Setup'
---

## Exercise 1: Create and export a configuration package

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

![Vendor info 01](media/vendor-info-01.png)

The following information is returned to you by Contoso’s super user:

![Vendor info 02](media/lab2_2_vendor_info_02.png)

### Tasks

1.  Create a configuration package.

2.  Assign tables and select fields.

3.  Export a configuration package to excel.

4.  Prepare data in excel.

### Steps

1.  Create a configuration package.

2.  From the main Business Central page in the black bar at the top of the page to the right, click the search icon. Type **Configuration Package**, then select the **Configuration Package** link. In the **Configuration Packages** page, click **New** to create a new configuration package.

3.  In the **Code** field, enter VENDOR.

4.  In the **Package Name** field, enter Vendor List.

5.  Assign tables and select fields.

6.  On the **Tables** section of the Config. Package Card, enter a new line
    as follows.

7.  Open the assist edit button to the right of the **Table ID** field.

8.  In the window that opens, select the **Vendor** table and click **OK**.

9.  Then press ENTER or TAB.

10. You will be asked to check related tables, click **No**.

11. Make sure the vendor table line is selected, select **Table** and then
    **Fields**.

12. On the field list page, first select **Clear Included**, to deselect the
    **Include Field** checkbox for all the fields.

13. Then select the **Include Field** checkbox for the following fields:

       1.  Name

       2.  Address

       3.  City

       4.  Phone No.

       5.  Currency Code

       6.  Language Code

       7.  Country/Region Code

       8.  Post Code

14. The **Validate Field** checkbox is automatically selected.

15. Click **Close**.

16. Export a configuration package to excel.

17. In the **Config. Package Card** page, select **Export to Excel**.

18. Click **Yes** to export the configuration package.

19. Prepare data in excel.

20. Open the exported excel file from the download folder.

21. Enter the information as provided by Contoso in the scenario description above, or use the provided Vendor Import.xlsx file.
   
22. Save the excel file.

23. Enter the information as provided by Contoso.

24. Save the excel file.

## Exercise 2: Import and apply a configuration package

### Scenario

When the vendor information is completed, you can now upload the vendor
information.

During this process, you want to make sure the data is validated and when
missing, the related tables will be automatically updated with newly provided
values.

### Tasks

1.  Import a configuration package from excel.

2.  Apply a configuration package.

3.  Resolve package errors.

### Steps

1.  Import a configuration package from excel.

2.  From the main Business Central page in the black bar at the top of the page to the right, click the search icon. Type **Configuration Package**, then select the **Configuration Package** link. In the **Configuration Packages** page, select the new configuration package for vendors and select **Manage** and then **Edit**.

3. In the **Config. Package Card** page select **Import from Excel**.

4.  Click **Choose…** and select the excel file.

5.  Click **Open**.

6.  In the preview page, select **Import**.

7.  Apply a configuration package.

8. In the **Config. Package Card** page, select **Apply Package**.

9.  Click **Yes**.

10. Resolve package errors.

11. In the **Config. Package Card** page, the vendor table line will show a
    number of errors.

12. Click on the number in the **No. of Package Errors** field.

13. In the error page, select the first record line and click **Show
    Error**.

14. Repeat for all the error records.

15. Click **OK**.

16. In the **Config. Package Card** page, select the vendor table line and
    select **Table** and then select **Fields**.

17. Select the **Create Missing Codes** check box, for the following fields:

       1.  Currency Code

       2.  Post Code

18. Click **Close**.

19. In the **Config. Package Card** page, select **Apply Package**.

20. Click **Yes**.

21. Click **OK**.

## Exercise 3: Import and apply a predefined package

### Scenario

For the further ease of the labs during the course, you will migrate the data
from the default CRONUS USA company within the database.

### Tasks

1.  Import and apply a predefined package.

### Steps

1.  Import and apply a predefined package.

2. In the **Configuration Packages** page, select **Actions**, then select **Import Predefined Package**.

3.  From the overview list, select the **Evaluation** package, containing
    the demo data.

4.  Click **OK**.

5. Select the imported configuration package, select **Apply Package**.

6.  Click **Yes**.

7.  A warning appears, where you select the **I understand, and want to
    continue** checkbox and click **OK**.

8.  Click **No** to any further questions.
