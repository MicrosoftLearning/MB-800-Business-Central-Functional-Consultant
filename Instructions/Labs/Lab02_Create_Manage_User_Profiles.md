---
lab:
  title: 'Lab 02: Create and manage user profiles'
  module: 'Manage users and implement security in Dynamics 365 Business Central'
  duration: 30 minutes
  level: 200
  islab: true
---


## Exercise: Create and manage user profiles


## Task 1: Make a copy of the profile without customization.

## Scenario
You are acting as the System Administrator responsible for configuring a new profile for Sales Managers in Business Central. The profile must be created by copying the standard SALES MANAGER profile and kept free of unnecessary customizations, ensuring it aligns with the organization’s requirements while maintaining consistency with the base role.


You will perform:

- Make a copy of the profile.

- Clear customization.


### Steps
1. Make a copy of the profile.

Select the Search icon in the top-right corner of the page, enter Profiles(Roles) and then choose the related link.

In the Profiles(Roles) page, select line with Profile ID field – SALES MANAGER, select Copy Profile on the menu.

Enter SALES CONTOSO to the Profile ID field.

Enter Sales Manager Contoso to the Display Name field.

Select OK.

2. Clear customization.

In the Profiles(Roles) page, select line with Profile ID field – SALES CONTOSO, select Edit.

Select Clear Customized pages on the Profile(Role) page.

Select Yes.

Select OK.



## Task 2: Set up a profile

## Scenario
The new profile must include a tailored Role Center and provide access to essential pages such as Customers, Sales Orders, and Reports. Sales Managers must not be allowed to add fields to any pages, ensuring controlled personalization and consistent data entry. Sections related to User Tasks and Job Queue Tasks are not required and should be removed, while the My Job Queue section must remain visible to support operational monitoring.


You will perform:

- Customize profile hide and show sections.

- Lock editing profile

### Steps
1. Customize profile hide and show sections.


2. Select the Search icon in the top-right corner of the page, enter Profiles(Roles) and then choose the related link.

3. In the Profiles(Roles) page, select line with Profile ID field – SALES CONTOSO, select Manage, Edit on the menu.

NOTE: New web page will be opened in the browser in Customize mode, in the left top corner will be the sign Customizing, Sales Manager Contoso.


4. Select the My Job Queue section, click on the red triangle at the top of the section, and select Show.

5. Scroll down to the end of the page.

6. Select the User Tasks section, click on the red triangle at the top of the section, and select Hide.

7. Select the Job Queue tasks section, click on the red triangle at the top of the section, and select Hide.


8. Select Done. Message Customization completed successfully. ... will be shown.

9. Close the current web page then return to the initial web page.


10. Lock editing profile


In the Profiles(Roles) page, select line with Profile ID field – SALES CONTOSO, select Manage, Edit on the menu.

Select Disable Personalization.



## Task 3: Assign a profile to the user.


## Scenario
You will assign a new configured profile to a designated user so that the Sales Manager experience reflects the intended layout, permissions, and navigation structure.


### Steps
1. Select the Search icon in the top-right corner of the page, enter User Settings and then choose the related link.

2. In the User Settings page, select line with your user, select Manage, Edit on the menu.

3. Select in the Role field – Sales Manager Contoso.


