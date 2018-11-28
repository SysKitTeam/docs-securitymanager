---
title: SysKit Security Manager 5.0.0 - Release Note
author: Petra Baresic
date: 04/12/2018 
description: This article describes what's new in the latest version of SysKit Security Manager.
---

SysKit Security Manager is a centralized SharePoint and Office 365 security reporting and management tool. It was created to help SharePoint global and site collection administrators control security in their SharePoint and Office 365 environments.

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

__Product version:__ 5.0.0  
__Build number:__      
__Release date:__ December 4, 2018  

## Features
* A new __Security Overview__ is available! Now you can get even better overview of your environment, both On-Prem and Online. SysKit Security Manager looks at your settings and activities and documents them through a set of security reports and health checks established by SysKit.The final score is based on the size of your Office 365 tenant/ Web Application and the sum of all the potential issues found. After the score is recalculated, the reports used for the calculation will be highlighted in color and you'll be able to drill down to reports to see more details.
* Together with the Security Overview we added some new permission and security reports: 
    * __Access Requests__ - Lists  all access requests on the selected subsite. 
    * __All Users__ – Shows all users from Azure Active Directory for SharePoint Online tenants or all users from connected site collections for on-premises web applications. 
    *  __Multi-Factor Authentication for Admins__ – Lists MFA information for site collection administrators. 
    * __External Sharing Settings__ – Lists sharing capabilities for site collections. 
    * __Customized Default Permission Levels__ – A list of default permission levels that are modified on specific site collections. 
    *  __Identical SharePoint Groups__ – SharePoint groups with identical users. 
    * __OneDrive Shared Items__ – Shows OneDrive items that have been shared.
* Now you can easily __jump between reports__ with drill actions or if you see on the report that permissions are not set correctly __switch to live view and manage permissions__. For example, by hovering a principals row in the Permission Matrix report you will now see a drill action which will help you to switch to the live view of our SharePoint Live explorer where you can manage permissions and more. Some other supported actions are navigating to the User Permission Details report and detailing only information about the user you clicked on, or finding out where external users have permissions.The reasoning behind this was to provide our users with a more manageable flow of navigating through extensive reporting features Security Manager offers. Read more about Security reports and available drill actions. 


## Improvements
* We improved OneDrive connection step in the connection wizard. 
* We added a notification to inform you when a new version of SysKit Security Manager is available to help users stay up to date with new features. 
* Some security reports now have a live version.
* We added a column grouping option which lets you group the report data by one or more columns and examine it from a different point of view. 
* We added the Snapshot Details report to help you troubleshoot load issues. 
* UX Improvements to the Stop Sharing OneDrive files action. 
* Improved reports filtering options.

## Bug Fix
* Fixed a bug where the Office 365 Group or Team URL was not recognized correctly and this cuased problems in the connection wizard.