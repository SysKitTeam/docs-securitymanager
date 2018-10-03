---
title: SysKit Security Manager 4.0.0 - Release Note
author: Petra Filipi 
date: 02/10/2018 
description: This article describes what's new in the latest version of SysKit Security Manager.
---

SysKit Security Manager is a centralized SharePoint and Office 365 security reporting and management tool. It was created to help SharePoint global and site collection administrators control security in their SharePoint and Office 365 environments.

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

__Product version:__ 4.0.0  
__Build number:__  983    
__Release date:__ October 4, 2018  

## Features
* __Discover and Connect to Microsoft Teams__ – SysKit Security Manager now offers support for Microsoft Teams. In the connection wizard you will be able to automatically find and [connect to all Microsoft Teams](#internal/how-to/connect-to-office-365) in your tenant. After you connect, you can explore all active and archived Teams in your tenant and their owners, members, guest users, and channels. You can also check the Global Settings report and control access to Teams in your organization. Available management actions are Clone, Update Team Settings, Add/Remove Owner, Add/Remove Member.

* __Connect to all OneDrive Accounts__ – if you are a Global Office 365 tenant administrator, you’ll have an option in the connection wizard to [connect to all OneDrive accounts](#internal/how-to/connect-to-office-365). After you connect you’ll be able to view all the OneDrive accounts within your tenant. Along with the names of the OneDrive users, you can also see their consumed storage levels, storage warning levels, and maximum allowed storage. The Activity column presents user activity and is calculated based on the last file activity of the OneDrive. 
The OneDrive screen gives you a general overview of your connected personal OneDrive accounts, as well as a report for each OneDrive account in which you can check the Sharing Details or Stop Sharing items (with everyone or just with external users).
At any time, you can disconnect all OneDrive accounts and remove administrator rights for all OneDrive accounts on the selected tenant using the Disconnect OneDrive action.

* __Group Reports__
  * __Group Members__ – shows all members of a selected SharePoint, Active Directory, or Security or Office 365 group.
  * __SharePoint Groups__ – shows all SharePoint groups and its members across the selected site collections.
  * __User Memberships__ – shows all the groups the selected principal is a member of.

* __Office 365 Groups Report__
  * __Office 365 Groups With Guests__ – shows all Office 365 groups that have guests or external users as owners or members.

* __Microsoft Teams Reports__
  * __Team Level Settings__ – shows Microsoft Teams settings by Team.
  * __Teams With Guests__ – shows all Microsoft Teams that have guests or external users as owners or members.

* __OneDrive Reports__
  * __Orphaned OneDrive__ – shows a list of OneDrive accounts whose owner is disabled or deleted from the Azure Active Directory.
  * __OneDrive With Guests__ – shows personal OneDrive accounts that have guests or external users with existing permissions.

* __Integrated Security__ – Now you can connect to your On-Premises environment using integrated credentials (the current Windows account credentials used for authentication). 

* __Settings Screen__ – Now you can modify options directly from the SysKit Security Manager interface.




