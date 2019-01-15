---
title: Permissions Reports Screen
description: >-
  This article describes how SysKit Security Manager permissions reports can
  help administrators track permissions and easily manage the SharePoint
  environment.
author: Petra Filipi
date: 14/05/2018
---

# permissions-reports-screen

The Permissions Reports screen contains a number of reports on SharePoint Permissions and Logical and Structural Reports.

To start exploring available SysKit Security Manager reports, take snapshot of your environment.

## Permission Reports

* **Permissions Matrix** – Shows all principals on a selected SharePoint object and which permission level each of them has.
* **Permission Level Usage** – Displays all the site collections where the selected permission level exists and if it is being used \(assigned to any principal\).
* **Unique Permissions** – Shows SharePoint objects \(sites, lists, items\) with unique permissions, e.g. objects with broken permission inheritance.

## User Reports

* **User Permissions Overview** – A summary of principals' permissions on the tenant. Shows site collections in which users have permissions, permissions that the users have as an individual, and the permissions that were given through a group. 
* **User Permissions Details** – Shows all permissions on all subsites inside a selected site collection for a specific user. The report shows permissions that a certain user has on each item within the particular site collection, along with the permissions that were given through a group. 

## Externally Shared

* **Externally Shared Content** – List of content in the tenant shared with external users, along with the external users it is shared with and the permissions they have on the content.
* **Externally Shared Content Matrix** – Shows externally shared content in the tenant hierarchy. Only the externally shared content is displayed.
* **Anonymous Access Links** –  A list of content in the tenant that has been shared with an anonymous guest link.
* **External Users** – Lists all external users in the tenant.

## Security Audit

* **Users with Privileged Access** – Shows all users with privileged access on the tenant or farm, such as farm and site administrators, or primary and secondary administrators, Users with Full Control / Full Read Web Application Policy, etc.

## Cleanup

* **Groups Without Permissions** – Lists all SharePoint groups that haven’t been assigned any permissions. This includes groups with ”Limited Access” that remained after their permissions on a specific item in the site collection were removed.
* **Groups With Disabled Owners** – Lists all SharePoint groups whose owners have been disabled in Active Directory.
* **Groups Without Users** – Lists all SharePoint groups without any members.
* **Orphaned Users** – Lists all tenant users that still have access to the tenant and are listed as site collection users, but have been disabled or deleted in Active Directory.
* **Users Without Permissions** – Lists all users that no longer have any permissions assigned, neither directly nor through any SharePoint groups. This also includes users with ”Limited Access” that have remained after their permissions on a specific item in the site collection were removed.
* **Site Collections With Disabled Administrators** – Crawls the selected site collections and lists those in which the primary or secondary administrator was disabled or deleted from Active Directory.

## Health Checks

* **Directly Assigned Permissions** – Shows users who have directly assigned permissions to securable objects within the selected site collections. Avoid granting permissions directly to individuals and work with groups instead.
* **Lists with Uniquely Secured Items** – Shows lists and libraries that contain list items with broken permissions inheritance.
* **Uniquely Secured List Items** – Shows all list items with broken permissions inheritance.

