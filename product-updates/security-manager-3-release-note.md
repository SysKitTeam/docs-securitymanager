---
title: SysKit Security Manager 3.0.0 - Release Note
author: Petra Filipi 
date: 18/07/2018 
description: This article describes what's new and improved in the latest version of SysKit Security Manager.
---

## We're excited to present SysKit Security Manager 3.0

SysKit Security Manager is centralized __SharePoint and Office 365 security reporting and management tool__. It was created to help SharePoint global and site collection administrators with controlling the security in their SharePoint and Office 365 environment.

Tool has gone through some changes since the last version. One of those changes is that entering password for SharePoint Online directly into SysKit Security Manager is no longer required. From now on, we are using the default sign in experience.
SysKit Security Manager requires [consent from a global administrator](internal/requirements/global-admin-consent). 
If you are an existing user you will be prompted to sign in and give global admin consent for __additional permissions__ for your existing connections.

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

__Product version:__ 3.0.0  
__Build number:__      
__Release date:__ July 18, 2018  


## Features
* __Automatic Discovery of Site Collections and Office 365 Groups for Global and Farm Administrators__ – If you are a global admin in Office 365 or a farm admin in SharePoint On-Premise, you will be able to automatically discover and connect to all site collections and Office 365 Groups in the tenant.
* __Ability to Import Site Collection List from File__– If you are a site collection admin or a farm admin you can connect to multiple site collections at one time by importing site collection URLs from a text file.  Site collection URLs in file must be newline separated. 
* __Ability to Take Partial Snapshots__ – Take snapshot option makes a snapshot of your environment. Now you can choose which site collections will be included in snapshot. Decide either to auto discover and load new site collections and Office 365 groups or manage site collections and Office 365 groups for snapshot from existing connections.
* __Security Audit Report__
    * __Users with Privileged Access__ – Shows all users with privileged access on the tenant or farm, such as farm and site administrators, or primary and secondary administrators, Users with Full Control / Full Read Web Application Policy, etc.
* __Health Checks Reports__
    * __Directly Assigned Permissions__– Shows users who have directly assigned permissions to securable objects within the selected site collections. Avoid granting permissions directly to individuals and work with groups instead.
    * __Lists with Uniquely Secured Items__ – Shows lists and libraries that contain list items with broken permissions inheritance.
    * __Uniquely Secured List Items__ – Shows all list items with broken permissions inheritance.

## Bug Fixes
* When attempting to connect to site collection using URL of a subsite, SysKit Security Manager displayed the following error: "_https://syskit.sharepoint.com/marketing/' is not a valid site collection or is not accessible._"
To avoid this error we improved validation of site collection links. Now you can connect to your site collection using subsite links or any URL that includes a valid URL of a site collection.
