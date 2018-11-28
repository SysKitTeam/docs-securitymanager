---
title: Overview Screen
description: In the Overview screen you can see at a glance if there are any potential issues in your environment.
author: Domagoj Hrestak
date: 04/12/2018
---

The __Overview__ screen is the starting screen of the SysKit Security Manager and features a dashboard of collected metrics and important information from your environment.

## Live Overview
Immediately upon connecting to a new tenant or an environment, Security Manager collects a number of important metrics and information regarding your Office 365 tenant or On-Prem environment and displays them in real time. Activities which are considered detrimental for environment health are highlighted in yellow, orange and red hues and are included in the final health score. To avoid long waiting and performance issues, information that is displayed with a camera icon is collected only when taking a snapshot.

## Snapshot Overview
Upon taking a snapshot Security Manager collects all of the available dashboard values so you can track your tenant summary information and health through time, potentially discovering a growing issue in your environment activities.

Environment health and potential issues are displayed via a score tile based on the size of your environment. Low score result means your environment is healthy and well-maintained.

## Analyze Results
Every collected metric will display a tooltip with more information when hovered over. Furthermore, every metric can be clicked on and the application will jump straight into a more detailed report view of the selected information, where you can analyze the results and fix any potential issues by using Security Manager drill actions for live permission management.

## Overview Tiles in Detail
All of the metrics with information regarding the reports they drill to.
### External Sharing
* __External Users__ – A list of all external users in the tenant.
* __Anonymous Access Links__ – List of content that has been shared with an anonymous guest link.
* __Site Collections With Enabled Anonymous links__ – Site collections with enabled anonymous access links sharing.
* __Site Collections With Enabled External Sharing__ – List of sharing capabilities for site collections.
### Items With Unique Permissions
* __Subsite__ – Report of all subsites with unique permissions.
* __Document Library__ – Report of all document libraries with unique permissions.
* __List__ – Report of all lists with unique permissions.
* __List Item__ – Report of all list items with unique permissions.
### Security
* __Customized Default Permission Levels__ – List of default permission levels that are modified on specific site collections.
* __Admins With Disabled MFA__ – Lists Multi-Factor-Authentication information for site collection administrators.
* __Site Collections Administrators__ – Lists users that are site collection administrators.
### OneDrive
* __OneDrive Close to Quota Limit__ – Lists OneDrive overview information including storage usage.
* __Orphaned OneDrive__ – List of OneDrive accounts whose owner is disabled or deleted in the Active Directory.
* __Inactive OneDrive__ – List of OneDrive storages which were not accessed in over three months.
* __Shared Items__ – List of OneDrive items that have been shared
* __Externally Shared Items__ – List of all content that is shared with external users.
#### Cleanup
* __Users Without Permissions__ – List of users who have not been assigned to any SharePoint or Security group and to whom no permissions have been directly assigned.
* __Groups Without Permissions__ – List of SharePoint groups that have not been assigned any permissions.
* __Groups With Disabled Owner__ – List of SharePoint groups whose owners have been disabled in the Active Directory.
* __Groups Without Users__ – List of SharePoint groups without any users.
* __Orphaned Users__ – List of users that are disabled or deleted but who had access to the tenant.
* __Site Collections With Disabled Owner__ – List of site collections and personal sites in which the primary administrator was disabled or deleted.
* __Identical SP Groups__ – SharePoint groups with identical users.
### Office 365 Groups & Teams
* __Office 365 Groups__ – List of all existing Office 365 Groups.
* __Microsoft Teams__ – List of all existing Office 365 Groups with Microsoft Teams.
* __Inactive Groups__ – List of groups which were not accessed in over three months.

