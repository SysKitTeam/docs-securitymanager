---
description: >-
  This article describes what's new in the latest version of SysKit Security
  Manager.
---

# SysKit Security Manager 7.1.0

This minor upgrade of SysKit Security Manager brings a variety of improvements in the Audit Log feature, a refreshed status bar, enhanced error handling, as well as numerous tweaks in the UX/UI. You'll also be happy to hear that we fixed some bugs. Read on for more information!

Try the latest version and [tell us what you think.](https://www.syskit.com/company/contact-us/)

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

**Product version:** 7.1.0  
**Build number:** 1897  
**Release date:** May 24, 2019

## Improvements

* We’ve **upgraded the Audit Log status bar**. You can see it in the lower right corner when SysKit Security Manager starts with the collection of Audit Log data. It gives you a detailed overview of how much data is currently being gathered from your tenant, from which workload, and how much data has been processed so far.  
* We’ve added two new status bar tabs: the **Audit Log Data Retention tab and Snapshot Data Retention tab**. They help you track the progress of Data Retention jobs being executed and the old audit log and snapshot data being deleted. You will notice them in the lower right corner when SysKit Security Manager runs the data retention jobs.  
* Added more understandable **guidelines on how to turn on and use Audit Logs** reporting in SysKit Security Manager. You will find more information when you go through the Connect Wizard as well as in the Settings page. Please keep in mind that Audit Logs reporting is supported for Office 365 environments only.  
* **Email alerts** that are sent by SysKit Security Manager when the disk is running out of space have received some **styling improvements**.  
* Improved the **Activities filter** look and feel on the Audit Logs Overview report.  
* Various UX/UI, objects naming and entry validation improvements. 

## Bug Fixes

* There was a problem with report filters being reset to a default setting once a new snapshot was started. Now, starting a new snapshot will not interfere with the filter settings of the currently generated report.  
* Resolved an issue where the following error was thrown: `Execution Timeout Expired. The timeout period elapsed prior to completion of the operation or the server is not responding. The backup or restore was aborted.`This happened when upgrading SysKit Security Manager to a newer version.  
* Fixed an issue where the following error would appear when trying to generate an Audit report for a Single Team: `System.Exception: Unknown team page url.`  
* Resolved issues when taking a snapshot for SharePoint 2010, which resulted in the following error: `Microsoft.SharePoint.Client.ServerException: Field or property "WebTemplate" does not exist.`   
* Resolved an issue which happened while loading permissions from a subsite, in the case when a SharePoint group was missing an owner. The following exception was thrown: `System.Data.SqlClient.SqlException: The INSERT statement conflicted with the FOREIGN KEY constraint "FK_LoadedGroupSettings_OwnerPrincipals.`  
* Fixed an issue with the default export location being erroneously set to the Audit Logs location, in the case when a custom Audit Logs location was set.  The export action now opens the user’s home folder, for example, C:\Users\John. 
* Fixed an issue where a group was automatically preselected when running the Add Owner or Add Member actions, in the case when the Office 365 Group was previously selected on the Single Group report.  
* Fixed a bug where the number of OneDrive sites was wrongly calculated and displayed in the Snapshot status bar in the case when the Discover & Load Everything option was selected.  
* Fixed an issue where reports would endlessly load results without ever showing them. The problem was due to a huge amount of data being processed and reaching a supported JSON file size limit. Now, the loading stops, and the following error is displayed: `Unexpected end of JSON input`  To avoid such cases, modify filters to show data for fewer SharePoint Objects.  
* Fixed an issue where saving a report set to the selected SharePoint Library would result in an error, in the case when a subscription was run.  

