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
* __Unique Permissions__ – 

## User Reports 

* __User Permissions Overview__ – A summary of principals' permissions on the tenant. Shows site collections in which users have permissions, permissions that the users have as an individual, and the permissions that were given through a group. 
* __User Permissions Details__ – Shows all permissions on all subsites inside a selected site collection for a specific user. The report shows permissions that a certain user has on each item within the particular site collection, along with the permissions that were given through a group. 

## Externally Shared

* __Externally Shared Content__ – List of content in the tenant shared with external users, along with the external users it is shared with and the permissions they have on the content.
* __Externally Shared Content Matrix__ – Shows externally shared content in the tenant hierarchy. Only the externally shared content is displayed.
* __Anonymous Access Links__ –  A list of content in the tenant that has been shared with an anonymous guest link.
* __External Users__ – Lists all external users in tenant

## Cleanup

* __Groups Without Permissions__ – Lists all SharePoint groups that haven’t been assigned any permissions. This includes groups with ”Limited Access” that remained after their permissions on a specific item in this site collection were removed.
* __Groups With Disabled Owners__ – Lists all SharePoint groups whose owners have been disabled in Active Directory.
* __Groups Without Users__ – Lists all SharePoint groups without any members.
* __Orphaned Users__ – ists all tenant users that still have access to the tenant and are listed as site collection user, but have been disabled or deleted in Active Directory.
* __Users Without Permissions__ – Lists all users that no longer have any permissions assigned, neither directly nor through any SharePoint groups. This also includes users with ”Limited Access” that have remained after their permissions on a specific item in this site collection were removed.
* __Site Collections With Disabled Administators__ – Crawls the selected site collections and lists those in which the primary or secondary administrator was disabled or deleted from Active Directory.





