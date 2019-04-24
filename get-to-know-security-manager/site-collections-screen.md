---
title: Site Collections Screen
description: Detailed overview of connected site collections.
author: Petra Filipi
date: 05/04/2018
---

# SharePoint Explorer Screen

The **SharePoint Explorer** screen gives you an overview of your connected site collections \(coloured red\) as well as connected Office 365 Groups site collections \(coloured blue\).

Track permissions changes in your environment using the [Compare wizard](../how-to/compare-permissions.md#compare-wizard).

## Permissions

The **Permissions** tab lets the site collection administrator explore SharePoint permissions in real time by simply navigating to the specific securable object. Use the tree on the left-hand side to navigate and expand to the desired SharePoint securable objects and view permissions details in the Permissions tab.

All management actions are contextually related to selected objects, which means users can select one or more users/groups to get actions related to the selected items.

**Securable objects that can be managed are:**

1. Users
2. SP \(SharePoint\) Groups
3. AD \(Active Directory\) Groups

### Available actions

* **Remove Tenant/ Web Application Connection** – Remove unwanted tenant or web application connections from SysKit Security Manager.
* **Refresh** – Reloads currently selected SharePoint object permission information or the entire permissions explorer tree.
* **View in SharePoint** – View and manage selected site content in your browser.
* **Edit Credentials** – Edit connected On-Premise site collection credentials.
* **Remove Connection** – Remove connection for either an Online or On-Premise site collection.
* **Site Collection Administrators** – Manage site collection admins. Change primary and secondary site collection administrators or entire site collection administrators group.
* **Break Inheritance** – Copies the parent permissions and then stops the permissions inheritance for the selected object. Any changes made to a parent site will not apply to the selected site in the future and vice versa.
* **Restore Inheritance** – Deletes all unique permissions and the selected securable object continues to inherit permissions from the parent site.
  * If you choose to restore the permission inheritance on a folder, you can choose an additional option to restore permission inheritance for all subitems as well.
  * Restoring permission inheritance on a subsite will also restore the permission inheritance on lists and list items on that subsite.
* **Grant Permissions** – Allows you to assign permissions to a user or a group on a selected SharePoint securable object with unique permissions.
* **Create Group** – Creates a new SharePoint group on the selected SharePoint object with unique permissions.
* **Go to Group** – Opens associated Office 365 Group for given Office 365 site collection.
* **Edit Settings** – Configures SharePoint group settings: name, owner, membership.
* **Edit** – Modifies assigned permission levels for a selected users or groups.
* **Remove** – Removes all previously granted permissions from a selected users. Users will still exist on this site collection but will no longer have any assigned permissions on this SharePoint object.
* **Copy** – Copy permissions and group memberships of the currently selected user to a different one. Source user’s permissions will not be changed in any way. Destination users will lose all previously assigned permissions and acquire every directly given permission and SharePoint group memberships as the source user.
* **Transfer** – Transfer permissions and group memberships from the currently selected user to a different one. Source user’s permissions will lose all previously directly assigned permissions and group memberships. Destination users will lose all previously assigned permissions and acquire every directly given permission and SharePoint group memberships as the source user.
* **Move to Group** – Removes directly assigned permissions from the selected users and adds them to a SharePoint group. Selected users will now inherit permissions through this group membership.
* **Copy to Group** – Allows you to directly add selected principals to the existing SharePoint groups.
* **Remove from Group** – Removes the selected users from the selected SharePoint group. Users will lose all permissions gained through this group membership.
* **Delete** – Deletes the selected users or groups from the entire site collection. Users or Active Directory/ Security group will no longer have any permissions assigned and will be deleted from the entire site collection.

## External Users on Site Collection

The **External Users on Site Collection** tab shows all the external users that have accessed your site collection.

## Access Requests

The **Access Requests** tab allows SharePoint site collection administrators to review and manage \(approve or decline\) access requests. If you approve the request, you can also specify the specific level of permission you’d like to assign to a user.

## Items with Unique Permissions

The **Items with Unique Permissions** lists all the objects with broken inheritance for the selected document library, list or folder.

* You can drill to the permissions report of the selected item to review its permissions.
* You can select one or more items and **Restore Inheritance** for all selected items at once.

## Anonymous Links

Use **Anonymous Links** tab to find out which documents or folders are shared to anonymous users with anonymous guest link and check link types and expiration dates.

