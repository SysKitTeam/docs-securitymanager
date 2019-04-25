---
title: Security Reports Screen
description: >-
  This article describes how SysKit Security Manager permissions reports can
  help administrators track permissions and easily manage the SharePoint
  environment.
author: Petra Filipi
date: 14/05/2018
---

# Security Reports Screen

The Security Reports screen contains a number of reports on SharePoint Permissions and Logical and Structural Reports.

There are two kinds of reports regarding the availability of data:

* those that can be viewed without creating a [snapshot](basics.md#snapshot) of your environment
* those that can be viewed only when a [snapshot](basics.md#snapshot) of your environment has been created

For detailed instructions on how to use Drill functionality and Filters, [see this article.](../how-to/use-filters-drill-and-column-chooser.md)

## Permission Reports

* **Permissions Matrix** – Shows all principals on a selected SharePoint object and which permission level each of them has.

  Permissions for multiple objects can be viewed at the same time. This report shows permissions for every kind of objects ranging from tenant to list item. Permissions for Groups, Teams and OneDrive objects can be viewed as well.

* **Permission Level Usage** – Displays all the site collections where the selected permission level exists and if it is being used \(assigned to any principal\).
* **Unique Permissions** – Shows SharePoint objects \(sites, lists, items\) with unique permissions, e.g. objects with broken permission inheritance.
* **Access Requests** - Lists all access requests across your subsites. 

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

## Audit Logs

* **Audit Logs Overview** – Lists all collected Audit logs.

  The following filters are available to help you find the needed information:

  * **Date Period** - Select between predefined values or click _Custom_ to open the Date and Time picker.
  * **Tenant** - In case you're connected to multiple tenants, select the one you want to display the audit logs for. By default, the first tenant on the list is selected.
  * **File, folder or site** - Use when your search is based on the knowledge of URL information. for example, if you want to see all activities on OneDrive sites, you can write _personal_ in this filter, since all such sites contain this word in the URL. Wildcards are also supported, but cannot be used as the first character in the filter.
  * **Activities** - By default, all the collected activities are displayed. By selecting a specific activities group or a single activity, the results are limited to the selection. To easily find wanted activities, use the **Search field.** To clear the selection, click the **Clear all to show results for all activities** button. To view all activities available for collection, use the **Can't find what you are looking for?** link on the bottom of the filter.
  * **Users** - By default, audit logs for all users are displayed. 

  The following actions are available:

  * **Generate** - When you change the above-mentioned filters, click the Generate button for them to be applied. 
  * **Schedule** - Add the Audit Logs Overview report along with the filter selection to a new or an existing report set to get it delivered automatically via email, or saved to a SharePoint document library.
  * **Export** - Export filtered audit logs to an excel file and save it to the desired location on your computer. The file comes with built-in sort and filter capabilities, enabling you to perform additional analysis of exported data.
  * **Search** - Searches for a string in all rows in the grid. Only rows that contain the input string are displayed, and the string itself is highlighted.

## Cleanup

* **Groups Without Permissions** – Lists all SharePoint groups that haven’t been assigned any permissions. This includes groups with ”Limited Access” that remained after their permissions on a specific item in the site collection were removed.
* **Groups With Disabled Owners** – Lists all SharePoint groups whose owners have been disabled in Active Directory. Supports live and snapshot data.
* **Groups Without Users** – Lists all SharePoint groups without any members. Supports live and snapshot data.
* **Orphaned Users** – Lists all tenant users that still have access to the tenant and are listed as site collection users, but have been disabled or deleted in Active Directory. Supports live and snapshot data.
* **Users Without Permissions** – Lists all users that no longer have any permissions assigned, neither directly nor through any SharePoint groups. This also includes users with ”Limited Access” that have remained after their permissions on a specific item in the site collection were removed.
* **Site Collections With Disabled Admins** – Crawls the selected site collections and lists those in which the primary or secondary administrator was disabled or deleted from Active Directory. Supports live and snapshot data.
* **Customized Default Permission Levels** – A list of default permission levels that are modified on specific site collections. Supports live and snapshot data.
* **Identical SP Groups** – SharePoint groups with identical users. Supports live and snapshot data.

## Health Checks

* **Directly Assigned Permissions** – Shows users who have directly assigned permissions to securable objects within the selected site collections. Avoid granting permissions directly to individuals and work with groups instead.
* **Lists with Uniquely Secured Items** – Shows lists and libraries that contain list items with broken permissions inheritance.
* **Uniquely Secured List Items** – Shows all list items with broken permissions inheritance.