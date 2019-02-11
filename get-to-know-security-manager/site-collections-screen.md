---
title: Site Collections Screen
description: Detailed overview of connected site collections.
author: Petra Filipi
date: 05/04/2018
---


# SharePoint Explorer

The **SharePoint Explorer** screen gives you an overview of your connected site collections \(coloured red\) as well as connected Office 365 Groups site collections \(coloured blue\).

Track permissions changes in your environment using the [Compare](compare-permissions.md) wizard.

## Permissions

The **Permissions** tab lets the site collection administrator explore SharePoint permissions in real time by simply navigating to the specific securable object. Use the tree on the left-hand side to navigate and expand to the desired SharePoint securable objects and view permissions details in the Permissions tab.

All management actions are contextually related to selected objects, which means users can **click on or hover over something to get a contextual menu** that offers actions related to the selected item.

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
* **Edit Group Settings** – Configures SharePoint group settings: name, owner, membership.
* **Edit Permissions** – Modifies assigned permission levels for a selected principal.
* **Remove Permissions** – Removes all previously granted permissions from a selected user. User will still exist on this site collection but will no longer have any assigned permissions on this SharePoint object.
* **Move to SharePoint Group** – Removes directly assigned permissions from the selected user and adds him to a SharePoint group. Selected user will now inherit permissions through this group membership.
* **Clone Permissions** – Source principal’s permissions will not be changed in any way. Destination principals will lose all previously assigned permissions and acquire every directly given permission and SharePoint group memberships as the source principal.
* **Transfer Permissions** – Source principal’s permissions will lose all previously directly assigned permissions and group memberships. Destination principals will lose all previously assigned permissions and acquire every directly given permission and SharePoint group memberships as the source principal.
* **Add to SharePoint Group** – Allows you to directly add selected principal to the existing SharePoint groups.
* **Remove User from Groups** – Removes the selected user from the selected SharePoint group. User will lose all permissions gained through this group membership.
* **Delete User** – Deletes the selected principal from the entire site collection. User or Active Directory/ Security group will no longer have any permissions assigned and will be deleted from the entire site collection.
* **Delete Group** – Deletes the selected SharePoint group from the entire site collection. This SharePoint group will no longer have any permissions assigned and will be deleted from the entire site collection.

## External Users on Site Collection

The **External Users on Site Collection** tab shows all the external users that have accessed your site collection.

## Access Requests

The **Access Requests** tab allows SharePoint site collection administrators to review and manage \(approve or decline\) access requests. If you approve the request, you can also specify the specific level of permission you’d like to assign to a user.

## Items with Unique Permissions

The **Items with Unique Permissions** lists all the broken inheritance objects in SharePoint. You can drill to the permissions report of the selected item to review its permissions.

## Anonymous Links

Use **Anonymous Links** tab to find out which documents or folders are shared to anonymous users with anonymous guest link and check link types and expiration dates.

