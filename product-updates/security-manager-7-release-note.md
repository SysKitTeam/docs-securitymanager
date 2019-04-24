---
title: SysKit Security Manager 7.0.0 - Release Note
author: Tomislav Sirovec
date: 23/04/2019
description: >-
  This article describes what's new in the latest version of SysKit Security
  Manager.
---

# SysKit Security Manager 7.0.0

This major upgrade of SysKit Security Manager brings you __bulk actions and Audit.__ Now, it is easier than ever to remove (or grant) access to as many users as you wish, and at the same time, the audit feature keeps track of everything that is done in the Tenant. There is no more sneaky access granting and hoping no one will notice! 

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

**Product version:** 7.0.0  
**Build number:** ????  
**Release date:** April 25, 2019

## Features

* __Bulk actions__ – The live permission explorer reports now support multiselect. What does that mean? Depending on the selected object/user certain actions are possible. E.g. You can now select as many users as you want and remove their permissions on a Site. Available actions are located on the action bar. For more information on all the available actions please see this article.  
* __Users section__ – Version 7 of SSM is now more than ever, focused on the user. We implemented a new Single User report. There are two main tabs which will be of interest:  
__1. Sites__ – Here you can find actions: 
  * Copy permissions - copy permissions and group memberships of the currently selected user to a different one, on the selected site(s).                   
  * Remove user – Remove the selected user from the selected site(s).  

  __2. Office 365 Groups & Teams__ – Here you can find actions: 
  * Copy Memberships – Which will copy Office 365 Group Memberships of the currently selected user to a destination user(s). 
  * Remove User – Remove the currently selected user from the Office 365 Groups & Teams. 

* __Audit__ - The __new Audit Logs Overview report__ lists __all activities__ in your Office 365 environment related to Azure Active Directory, SharePoint, Microsoft Teams, Office 365 Groups and OneDrive. Use the advanced search capabilities to quickly find specific activities, __export the report to an excel file__ with added sort and filter options, or __add the report to a schedule__ and get it __automatically delivered via email.__   

* The __new Audit tabs__ available throughout the application give you a __custom view of activities related to the current context.__ For example, if you are currently looking into a specific Single Team, the available Audit tab will only display activities performed in the selected Team - e.g. Team Created, Added members to the team, etc. __Audit tabs are available on all objects in SysKit Security Manager__ - SharePoint objects, Office 365 Groups, Microsoft Teams, OneDrive, and Users.  

  To find out how to start collecting audit logs with SysKit Security Manager, follow this link.  

  For a better understanding of Microsoft's audit logs, please read our Audit blog post. 

* __Data Retention__ - Free up your disk and database space by enabling __data retention for Snapshots and Audit Logs.__ Once you define how long you want to keep your data,SysKit Security Manager will take care of the rest and remove old data __automatically.__ To make sure you collect all of your audit logs, SysKit Security Manager monitors the disk usage and sends you an __email alert, once the disk gets close to being full.__  
For more information about all data retention settings, navigate to this article.  

## Improvements

* __Teams, Office 365 Groups and OneDrive__ reports no longer have a tree view in the navigation. Also, all of the reports from the Security reports section have been moved to their corresponding sections in the main navigation.  
* New __Orphaned Teams and Orphaned Office 365 Groups reports__ – The reports will show you which Teams and/or Groups don’t have any active owners. This means that all owners are disabled in Azure Active Directory or there are no owners at all. 
* __Improved status bar!__ We have expanded on the pool of information we provide you with, while taking a snapshot. Also, every major action you do (e.g. copy permissions) will have its own tab in the status bar from where you can track its progress. 
* __New and improved grid!__ Every column is now searchable and has a filter. This should help in finding whatever the end user is interested in
* We have __improved the way SSM pulls data from Microsoft.__ GraphAPI calls are now also improved - with the result being a more stable and throttle free application.  
* __Restore inheritance option__ in the Items with Unique Permissions report in SharePoint Explorer is now available. Instead of restoring the inheritance one item at a time, you can now do it on the entire list or document library.   
* Root node is no longer disabled on the Directly Assigned Permissions report. 
* We improved the way __Access Request__ is loaded. No change for the end user should be visible.    
* SP Objects filter is renamed to __Tenants__ when there is only one object level to show.
* When taking a snapshot, we no longer classify Access denied and forbidden messages as an error.
* Various UI and UX improvements.  

## Bug fix

* There was a problem with a timestamp when exporting the External users and External Sharing Settings report. That is now fixed.  
* On the OneDrive Overview report, sorting by Activity column is now fixed. 
* When inputting credentials, that is, the login name, we fixed a bug where the pointer would freely jump to the end. 
* We fixed a bug when using the SQL Authentication to connect to the database. 
=======
## Improvements

## Bug fix


