---
title: SysKit Security Manager 5.0.0 - Release Note
author: Petra Baresic
date: 04/12/2018 
description: This article describes what's new in the latest version of SysKit Security Manager.
---

We are glad to announce that we released the new version of SysKit Security Manager today.
This major upgrade brings security overview capabilities to your environment and a lot of new and improved security reports.

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

__Product version:__ 5.0.0  
__Build number:__      
__Release date:__ December 4, 2018  

## Features
* The new [__Security Overview__](#internal/get-to-know-security-manager/overview-screen) is available! Now you can get even better visibility into your environment, both On-Prem and Online. SysKit Security Manager looks at your settings and activities and documents them through a set of security reports and health checks developed by SysKit. The final score is based on the size of your Office 365 tenant/web application and the sum of all the potential issues found. After the score is recalculated, the reports used for the calculation will be highlighted in color, and you'll be able to drill down into reports that offer more details. 
* Together with the Security Overview we added some new permission and [security reports](#internal/get-to-know-security-manager/permissions-reports-screen):
    * __Access Requests__ - Lists  all access requests on the selected subsite. 
    * __All Users__ – Shows all users from Azure Active Directory for SharePoint Online tenants or all users from connected site collections for on-premises web applications. 
    * __Multi-Factor Authentication for Admins__ – Lists MFA information for site collection administrators. 
    * __External Sharing Settings__ – Lists sharing capabilities for site collections. 
    * __Customized Default Permission Levels__ – A list of default permission levels that are modified on specific site collections. 
    * __Identical SharePoint Groups__ – SharePoint groups with identical users. 
    * __OneDrive Shared Items__ – Shows OneDrive items that have been shared.
* Now you can easily __jump between reports__ with drill actions or if you see on the report that permissions are not set correctly __switch to live view and manage permissions__. For example, by hovering a principals row in the Permission Matrix report you will now see a drill action which will help you to switch to the live view of our [SharePoint Explorer Screen](#internal/get-to-know-security-manager/site-collections-screen) where you can manage permissions and more. Some other supported actions are navigating to the User Permission Details report and detailing only information about the user you clicked on, or finding out where external users have permissions.The reasoning behind this was to provide our users with a more manageable flow of navigating through extensive reporting features Security Manager offers. Read more about [security reports](#internal/get-to-know-security-manager/permissions-reports-screen) and available drill actions.

## Improvements
* We improved the OneDrive connection step in the [connection wizard](#internal/how-to/connect-to-office-365). Granting administrator rights to OneDrive in the connection wizard using the option __Connect to all OneDrive accounts__, now correctly checks if the current user already has site collection administrator permissions through a SharePoint or a Security Group. When disconnecting OneDrive from Security Manager and choosing to remove all site collection administrator rights, only directly given permissions are removed.
The connection wizard performance has been improved while checking and giving permissions to OneDrive accounts, but the finishing step of the wizard can still take a while for large numbers of users with OneDrive.
* We added a notification feature to inform you when a new version of SysKit Security Manager is available, helping you stay up to date with new features. 
* Some [security reports](#internal/get-to-know-security-manager/permissions-reports-screen) now have a live version.
* We added a column grouping option, which lets you group the report data by one or more columns and examine it from a different point of view
* We added the Snapshot Details report to help you troubleshoot load issues.
* The Stop Sharing OneDrive files action features UX improvements.
* We improved report filtering options.

## Bug Fix
* We fixed a bug that caused the Office 365 Group or Team URL to not be recognized correctly, which caused problems in the connection wizard.
