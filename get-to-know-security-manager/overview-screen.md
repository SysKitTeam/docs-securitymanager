---
title: Overview Screen
description: In the Overview screen you can see at a glance if there are any potential issues in your environment.
author: Domagoj Hrestak
date: 04/12/2018
---

The __Overview__ screen is the starting screen of the SysKit Security Manager. It features a dashboard of collected metrics and important information from your environment.

## Live Overview
Immediately upon connecting to a new tenant or an environment, Security Manager collects a number of important metrics and information regarding your Office 365 tenant or On-Prem environment and displays them in real time. To avoid long waiting times and performance issues, information that is displayed with a camera icon is collected only when taking a snapshot. 

Clicking on the refresh button in the upper-right part of the overview will refresh it with the latest information and recalculate your score.

## Snapshot Overview
Upon taking a snapshot Security Manager collects all the available dashboard values. So you can track your tenant summary information and health through time, potentially discovering a growing issue in your environment activities.

## Score
Environment health and potential issues are displayed via a score tile based on the size of your environment. A low score means your environment is healthy and well-maintained.

Activities which are considered detrimental to environment health are highlighted in yellow, orange and red and are included in the final health score. Hovering over the score tile will highlight all the values which are taken in consideration when calculating the final score.

## Analyze Results
Every collected metric will display a tooltip with more information when hovered over. Furthermore, every metric can be clicked on and the application will jump straight into a more detailed report view of the selected information. Here you can analyze the results and fix any potential issues by using Security Manager drill actions for live permission management.

## Overview Tiles in Detail
Here you can find a list of all the tile categories and what kind of information they represent. For detailed information about the reports they describe head over to the [__Security Reports__](#internal/get-to-know-security-manager/permissions-reports-screen) section.

Underneath the score tile you can find a list of general environment information. When a tile value is displayed as a fraction, the first number represents how many objects of the described type are connected in Security Manager and the second number is the total number of objects in your environment. This information is only present in the live overview.

* __External Sharing__ – Information about the number of external users and sharing capabilities of your site collections.

* __Items With Unique Permissions__ – SharePoint items with unique permissions.

* __Security__ – Site Collection Administrators information and default permission levels that have been modified.

* __OneDrive__ – Find out more about your users OneDrive activities, including storage use, inactivity periods, externally shared items and more.

* __Cleanup__ – Information which directly influences your score calculation. Such as orphaned users, groups without users, identical SharePoint groups and disabled owners for site collections.

* __Office 365 Groups & Teams__ – Total number of Office 365 Groups and groups associated with Microsoft Teams.

