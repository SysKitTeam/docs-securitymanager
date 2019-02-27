---
title: SysKit Security Manager 6.0.0 - Release Note
author: Tomislav Sirovec
date: 19/02/2019
description: >-
  This article describes what's new in the latest version of SysKit Security
  Manager.
---

# SysKit Security Manager 6.0.0

This major upgrade of SysKit Security Manager brings automation to the table! Scheduled reports and scheduled snapshots are now available. Also, take a detailed look of all the improvements we made.

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

**Product version:** 6.0.0  
**Build number:** 1467  
**Release date:** February 19, 2019

## Features

* **Scheduled Reports** – you can now schedule and send security reports. This feature allows you to select one or more reports to be sent to you at any time and frequency you want – daily, weekly, monthly or after a scheduled snapshot. Alongside the email, the report can be saved to a SharePoint library as well. 
  * A new screen, [Scheduled Reports](../get-to-know-security-manager/scheduled-reports-screen.md), was added on the main navigation. You can add a new report into an existing report set. A schedule option is also available from any report on the Security Reports screen. This will add currently selected reports to a new report or into an existing one, depending on your choice.
* [Scheduled Snapshots](../installation/installation-guide.md) – when upgrading to v6, we suggest selecting the advanced installation \(installation guide\) of the application. It allows you to take scheduled snapshots while the application is not running. A dedicated SQL Server database and service account is required.
* We added a **Large Lists report**. It will show you any lists and libraries that have more than 4000 items.

## Improvements

* There are now two [types of installation](../installation/installation-guide.md) available.
  * **Default installation type** - no additional configuration is required and it's suitable for most users. 
  * **Advanced type** - If you want to take scheduled snapshots and reports while the application is not running choose this option. It is a type of installation which requires a dedicated SQL Server database and a service account. 
* We added a **column chooser** on the Teams Overview report, which allows you customization of the way your reports look. Just click on the column icon on the right side of the report. There you can manage which columns you want to see. For instance, you can disable any of the available columns, such as the Privacy or Created On column and easily return them if you’ll ever need them. We also added a new column in the Teams overview – Site URL, so you now have an insight in URLs from all of your Teams.
* Additional [settings options](../get-to-know-security-manager/settings-screen.md) have been added to SSM, so you can easily find options that you wish to change. The three main categories are General, Reporting and Snapshot. We have also added a back button so you can quickly continue where you have left off.
* We redesigned the **Take Snapshots dialogue**. The new design enables you to easily pick the type of snapshot and what will be included in the snapshot.
* We moved the **Snapshots screen button** down on the main navigation – it is now above the Scheduled Reports and Settings buttons. From the Snapshots screen, you can now access the Snapshot Schedule option.
* On the [OneDrive screen](https://github.com/SysKitTeam/docs-securitymanager/tree/b27dc2ed5050f6bcf938ebef9822a31b27b6463c/product-updates/..get-to-know-security-manager/onedrive-screen.md), hover the mouse over an user and the button to remove access from a single user’s OneDrive will appear.
* The **OneDrive Shared Items** report is no longer organized in a SharePoint object hierarchy. Now, it immediately shows all shared objects of each user’s OneDrive.
* We improved the UX when connecting to and disconnecting from peoples OneDrive’s. If you decide you no longer wish to manage OneDrive \(or when deleting the SSM application\) these permissions can be removed by clicking the Remove Access button on top of the screen of the One Drive tab.
* You can now **export** details of your snapshots in .xlsx format. On the snapshots tab, select a snapshot and click the Snapshot Details button.
* On the Microsoft Teams tab, manage actions are improved. Clone Team, Update Team Settings, Remove Team and Delete Team options are available from the main navigation when you select a specific team, and on the general report when you hover over the teams.
* For easier management, on both the Office 365 Groups and Microsoft Teams screen, all the users \(Owners, Members and Guests\) are now shown together in a single column. When you select a specific team or group, in the Role column you can now see the role of your members.
* On the [Overview Screen](../get-to-know-security-manager/overview-screen.md) a progress loading bar has been added.
* When you first start the application, a short guide will take you through all the new features.
* The number of owners, members and guests are now shown on the tenant overview for both Office 365 Groups and Microsoft Teams reports.
* When the Connect wizard is finished, the app will automatically trigger a snapshot and, if there is no snapshot detected, load the selected site collections, Office 365 Groups, Teams or OneDrive accounts. In this way you will have your report data ready as soon as possible.
* Improved UI for adding the on premises site collections manually.
* In the **Microsoft Teams section**, we added **new columns** in the Channels tab. You can now see the URL and Email of your Teams’ channels.
* Deleted SharePoint sites won’t be shown in the app. After you make a snapshot, deleted site collections and groups won’t appear anymore.

## Bug fix

* Fixed the alphabetical order on all reports.
* Fixed a bug where OneDrive's were being shown on Unique Permissions and Uniquely Secured List Items reports, while in fact they were not supposed to be.
* Minor bug fixes and improvements.
* Fixed a bug when trying to load a site collection. The received error was: 

```text
“Violation of PRIMARY KEY constraint 'PK_SharePointObjectPendingAccessRequests'. Cannot insert duplicate key in object 'dbo.SharePointObjectPendingAccessRequests'”
```

* When connecting to On-Premises site collections using SharePoint configuration database, error was happening when using custom credentials.

