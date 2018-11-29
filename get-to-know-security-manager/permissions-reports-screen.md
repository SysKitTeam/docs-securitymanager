---
title: Permissions Reports Screen
description: This article describes how SysKit Security Manager permissions reports can help administrators track permissions and easily manage the SharePoint environment.
author: Petra Filipi
date: 14/05/2018
---
The Permissions Reports screen contains a number of reports on SharePoint Permissions and Logical and Structural Reports.

To start exploring available SysKit Security Manager reports, take snapshot of your environment.

## Permission Reports

* __Permissions Matrix__ – Shows all principals on a selected SharePoint object and which permission level each of them has.
* __Permission Level Usage__ – Displays all the site collections where the selected permission level exists and if it is being used (assigned to any principal).
* __Unique Permissions__ – Shows SharePoint objects (sites, lists, items) with unique permissions, e.g. objects with broken permission inheritance.

## User Reports 

* __User Permissions Overview__ – A summary of principals' permissions on the tenant. Shows site collections in which users have permissions, permissions that the users have as an individual, and the permissions that were given through a group. 
* __User Permissions Details__ – Shows all permissions on all subsites inside a selected site collection for a specific user. The report shows permissions that a certain user has on each item within the particular site collection, along with the permissions that were given through a group. 
* __Users with Privileged Access__ – Shows all users with privileged access on the tenant or farm, such as farm and site administrators, or primary and secondary administrators, Users with Full Control / Full Read Web Application Policy, etc.

## Group Reports

* __Group Members__ – Shows all members of a selected SharePoint, Active Directory, or Security or Office 365 group.
* __SharePoint Groups__ – Shows all SharePoint groups and its members across the selected site collections.
* __User Memberships__ – Shows all the groups the selected principal is a member of.

## Externally Shared

* __Externally Shared Content__ – List of content in the tenant shared with external users, along with the external users it is shared with and the permissions they have on the content.
* __Externally Shared Content Matrix__ – Shows externally shared content in the tenant hierarchy. Only the externally shared content is displayed.
* __Anonymous Access Links__ –  A list of content in the tenant that has been shared with an anonymous guest link.
* __External Users__ – Lists all external users in the tenant.

## Cleanup

* __Groups Without Permissions__ – Lists all SharePoint groups that haven’t been assigned any permissions. This includes groups with ”Limited Access” that remained after their permissions on a specific item in the site collection were removed.
* __Groups With Disabled Owners__ – Lists all SharePoint groups whose owners have been disabled in Active Directory.
* __Groups Without Users__ – Lists all SharePoint groups without any members.
* __Orphaned Users__ – Lists all tenant users that still have access to the tenant and are listed as site collection users, but have been disabled or deleted in Active Directory.
* __Users Without Permissions__ – Lists all users that no longer have any permissions assigned, neither directly nor through any SharePoint groups. This also includes users with ”Limited Access” that have remained after their permissions on a specific item in the site collection were removed.
* __Site Collections With Disabled Administrators__ – Crawls the selected site collections and lists those in which the primary or secondary administrator was disabled or deleted from Active Directory.

## Health Checks

* __Directly Assigned Permissions__ – Shows users who have directly assigned permissions to securable objects within the selected site collections. Avoid granting permissions directly to individuals and work with groups instead.
* __Lists with Uniquely Secured Items__ – Shows lists and libraries that contain list items with broken permissions inheritance.
* __Uniquely Secured List Items__ – Shows all list items with broken permissions inheritance.

## Microsoft Teams Reports

* __Team Level Settings__ – Shows Microsoft Teams settings by Team.
* __Teams With Guests__ – Shows all Microsoft Teams that have guests or external users as owners or members.

## Office 365 Groups Reports
__Office 365 Groups With Guests__ – Shows all Office 365 gGroups that have guests or external users as owners or members.

## OneDrive Reports
* __Orphaned OneDrive__ – Shows a list of OneDrive accounts whose owner is disabled or deleted from the Azure Active Directory.
* __OneDrive With Guests__ – Shows personal OneDrive accounts that have guests or external users with existing permissions.


## Drill Functionality
Most of the reports are interconnected between each other and with the rest of the application. You can drill from one to the other by using the drill functionality.  
The drill functionality is available when you hover or select a row in a report and is denoted with a recognizable drill icon. Depending on the report different options to drill will be available. Different rows may also have different drill options and lead to different parts of the application.  

I.e. the Permissions Matrix report allows the following:
- if a SharePoint object is selected - switching to live permissions on the SharePoint Explorer screen to allow permission management on the object in question 
- if a user is selected 
    - switching to the User Permissions Details Report
    - switching to live permissions on the SharePoint Explorer screen to allow permission management on the object where the user has permissions
