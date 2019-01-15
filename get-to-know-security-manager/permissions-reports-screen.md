---
title: Security Reports Screen
description: >-
  This article describes how SysKit Security Manager permissions reports can
  help administrators track permissions and easily manage the SharePoint
  environment.
author: Petra Filipi
date: 14/05/2018
---

# permissions-reports-screen

The Security Reports screen contains a number of reports on SharePoint Permissions and Logical and Structural Reports.

There are two kinds of reports regarding the availability of data:

* those that can be viewed without creating a [snapshot](../get-to-know-security-manager/basics.md#snapshot) of your environment
* those that can be viewed only when a [snapshot](../get-to-know-security-manager/basics.md#snapshot) of your environment has been created

## Filters

Before you can view the report data you will need to configure the report filters. The available filters will depend on the selected report. All reports will have at least the Snapshot filter and the SharePoint Objects filter available.

* **Snapshot** - The Snapshot Filter allows you to view the report for a specific snapshot that you have taken.  It also contains the Live entry, which can be used to generate a report without creating a snapshot. Because of the complexity of some reports, not all of them support the Live option.
* **SharePoint Objects** - This is a complex filter that supports the picking of objects from an Office 365 tenant or SharePoint On-Premises on multiple levels. Depending on the report in question it will ask you to choose either a tenant/On-Premise web application or site collections from a tenant. All of the connected site collections will be shown in this filter including Office 365 Groups, Teams and OneDrive site collections. The **Permissions Matrix** and the **Externally Shared Content Matrix** reports use a more advanced configuration of this filter and you can choose a specific securable object in the SharePoint hierarchy.  So, to generate the **Permissions Matrix** report for a specific list, you would drag the Filter By slider to _Lists_ and select an object in each of the categories: Tenants, Sites, Subsites, Lists.
* **Content Level** - The Content Level filter lets us choose which types of objects we want to include in the generated report. It is called **Content Level** because the selection of the filter determines the lowest level for which the report will be generated.  For example, choosing **Subsites** in the **Permissions Matrix** will result in a report that contains data down to the subsites level. Permission data for lists and list items will not be included. 
* **Principals** - The Principals filter is used to filter by principals. Principals include: 
  * users
  * security groups, Office 365 Groups
  * SharePoint Groups
  * special groups that represent _Sharing Links_
    * People in the organization with a view sharing link
    * People in the organization with an edit sharing link
    * Anyone with an anonymous view sharing link
    * Anyone with an anonymous edit sharing link
    * Specific people with a sharing link
* **Securable Objects** - By default, reports that show permissions are generated only for objects that have unique permissions or the directly selected objects in the SharePoint Objects filter. Any child objects will have their permissions shown only if they are uniquely secured. This is so as to avoid an explosion of report data because each and every object above or equal to the _Content Level_ filter would be shown along with the associated permissions. If you do wish to see each and every child object along with their permissions \(which would be the same as the parent object by definition\) you can use this filter to modify the report behavior.

## Drill Functionality

Most of the reports are interconnected between each other and with the rest of the application. You can drill from one to the other by using the drill functionality.  
The drill functionality is available when you hover or select a row in a snapshot report and is denoted with a recognizable drill icon. Depending on the report different options to drill will be available. Different rows may also have different drill options and lead to different parts of the application.

For example the **Permissions Matrix** report allows the following:

* if a SharePoint object is selected - switching to live permissions on the **SharePoint Explorer** screen to allow permission management on the object in question 
* if a user is selected 
  * switching to the **User Permissions Details** Report
  * switching to live permissions on the **SharePoint Explorer** screen to allow permission management on the object where the user has permissions

## Permission Reports

* **Permissions Matrix** – Shows all principals on a selected SharePoint object and which permission level each of them has.

  Permissions for multiple objects can be viewed at the same time. This report shows permissions for every kind of objects ranging from tenant to list item. Permissions for Groups, Teams and OneDrive objects can be viewed as well.

* **Permission Level Usage** – Displays all the site collections where the selected permission level exists and if it is being used \(assigned to any principal\).
* **Unique Permissions** – Shows SharePoint objects \(sites, lists, items\) with unique permissions, e.g. objects with broken permission inheritance.
* **Access Requests** - Lists  all access requests across your subsites. 

## User Reports

* **User Permissions Overview** – A summary of principals' permissions on the tenant. Shows site collections in which users have permissions, permissions that the users have as an individual, and the permissions that were given through a group. 
* **User Permissions Details** – Shows all permissions on all subsites inside a selected site collection for a specific user. The report shows permissions that a certain user has on each item within the particular site collection, along with the permissions that were given through a group. This report can show every object in your environment to which a specified user or users have access to. This includes all SharePoint objects, Groups and Teams objects and OneDrive files.  
* **Users with Privileged Access** – Shows all users with privileged access on the tenant or farm, such as farm and site administrators, or primary and secondary administrators, Users with Full Control / Full Read Web Application Policy, etc. Supports live and snapshot data.
* **All Users** – Shows all users from Azure Active Directory for SharePoint Online tenants or all users from connected site collections for on-premises web applications. Supports live and snapshot data.
* **Multi-Factor Authentication for Admins** – This report shows which site collection admins have multi-factor authentication enabled. It is recommended that all users with privileged access have Multi-Factor Authentication enabled. [Possible MFA states are](https://social.msdn.microsoft.com/Forums/azure/en-US/46d1e71e-f98a-4e97-94f8-11621c3385d8/mfa-status-enabled-enforced?forum=windowsazureactiveauthentication):
  * **Disabled** - This is the default state for a new user not enrolled in multi-factor authentication.
  * **Enabled** - The user has been enrolled in multi-factor authentication, but has not completed the registration process. They will be prompted to complete the process the next time they sign in.
  * **Enforced** - The user may or may not have completed registration. If they have completed the registration process then they are using multi-factor authentication. Otherwise, the user will be prompted to completer the process at next sign-in. In non-browser apps \(such as Outlook etc.\) will not work until app passwords are created and entered into the non-browser apps.

    In order to use this report the following prerequisites need to be satisfied:

  * Powershell version 3.0. or newer
  * Latest MSOnline powershell module installed - can be installed by running the following powershell commandlet: Install-Module MSOnline

## Group Reports

* **Group Members** – Shows all members of a selected SharePoint, Active Directory, or Security or Office 365 group. Supports live and snapshot data.
* **SharePoint Groups** – Shows all SharePoint groups and its members across the selected site collections.
* **User Memberships** – Shows all the groups the selected principal is a member of.

## External Sharing

* **Externally Shared Content** – List of content in the tenant shared with external users, along with the external users it is shared with and the permissions they have on the content.
* **Externally Shared Content Matrix** – Shows externally shared content in the tenant hierarchy. Only the externally shared content is displayed. This report identifies who has access to your files outside of your organization including the permissions they have on your files. This includes all SharePoint objects, Groups and Teams objects and OneDrive files. 
* **Anonymous Access Links** –  A list of content in the tenant that has been shared with an anonymous guest link.
* **External Users** – Lists all external users in the tenant. Supports live and snapshot data.
* **External Sharing Settings** – Lists sharing capabilities for site collections. Supports live and snapshot data.

## Cleanup

* **Groups Without Permissions** – Lists all SharePoint groups that haven’t been assigned any permissions. This includes groups with ”Limited Access” that remained after their permissions on a specific item in the site collection were removed.
* **Groups With Disabled Owners** – Lists all SharePoint groups whose owners have been disabled in Active Directory. Supports live and snapshot data.
* **Groups Without Users** – Lists all SharePoint groups without any members. Supports live and snapshot data.
* **Orphaned Users** – Lists all tenant users that still have access to the tenant and are listed as site collection users, but have been disabled or deleted in Active Directory. Supports live and snapshot data.
* **Users Without Permissions** – Lists all users that no longer have any permissions assigned, neither directly nor through any SharePoint groups. This also includes users with ”Limited Access” that have remained after their permissions on a specific item in the site collection were removed.
* **Site Collections With Disabled Adminis** – Crawls the selected site collections and lists those in which the primary or secondary administrator was disabled or deleted from Active Directory. Supports live and snapshot data.
* **Customized Default Permission Levels** – A list of default permission levels that are modified on specific site collections. Supports live and snapshot data.
* **Identical SP Groups** – SharePoint groups with identical users. Supports live and snapshot data.

## Health Checks

* **Directly Assigned Permissions** – Shows users who have directly assigned permissions to securable objects within the selected site collections. Avoid granting permissions directly to individuals and work with groups instead.
* **Lists with Uniquely Secured Items** – Shows lists and libraries that contain list items with broken permissions inheritance.
* **Uniquely Secured List Items** – Shows all list items with broken permissions inheritance.

## Office 365 Groups Reports

**Office 365 Groups With Guests** – Shows all Office 365 Groups that have guests or external users as owners or members.

## Microsoft Teams Reports

* **Team Level Settings** – Shows Microsoft Teams settings by Team. Team settings are showed for all Microsoft Teams on a selected tenant.
* **Teams With Guests** – Shows all Microsoft Teams that have guests or external users as owners or members.

## OneDrive Reports

* **Orphaned OneDrive** – Shows a list of OneDrive accounts whose owner is disabled or deleted from the Azure Active Directory. Supports live and snapshot data.
* **OneDrive With Guests** – Shows personal OneDrive accounts that have guests or external users with existing permissions.
* **OneDrive Shared Items** – Shows OneDrive items that have been shared. Report can show shared items across multiple OneDrive storages at the same time. For detailed information about permissions on specific shared files this report has built-in drill functionality to Permissions Matrix report.

