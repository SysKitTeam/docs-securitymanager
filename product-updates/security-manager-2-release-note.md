---
title: SysKit Security Manager 2.0.0 - Release Note
date: 16/05/2018
description: >-
  This article describes what's new and improved in the latest version of SysKit
  Security Manager.
---

# security-manager-2-release-note

SysKit Security Manager is centralized **SharePoint and Office 365 security reporting and management tool**. It was created to help SharePoint site collection administrators with controlling the security in their SharePoint and Office 365 environment.

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

**Product version:** 2.0.0  
**Build number:** 607  
**Release date:** May 16, 2018

## Features

* **SharePoint Online and On-Premises Snapshots** are now available in SysKit Security Manager! In addition to being able to manage SharePoint Online and On-Premises permissions, you can now take snapshots of all your site collections and Office 365 groups. This is required in order to use the more advanced **Permission Reports.**
* Use the **Permissions Reports** screen to gather valuable information about structure, granted permissions, broken permissions inheritance, and more. We broke them down into four categories. For detailed information on every report see [this article](security-manager-2-release-note.md#internal/get-to-know-security-manager/permissions-reports-screen).
  * **Permissions reports:**

    Auditing SharePoint permissions can be a complex and time-consuming task. SysKit Security Manager allows administrators to drill down and view all permissions, explore permissions history, and create site and user specific reports.

  * **User reports:**

    These reports can either give you a **summary** or a **detailed view** on the permissions that a principal has within a particular site collection.

  * **Externally Shared:**

    A handful of reports concerning externally shared content and external users.  
    They will show you which content is shared with external users, and what permissions those users have on the content. A list of content shared via anonymous links, and even a list of all unlicensed \(external\) users on your tenant.

  * **Cleanup:**

    It is a known thing that SharePoint gets cluttered. Users get disabled, permissions are removed, SharePoint groups lose their members and so on. When cases like this happen, it is recommended to manage and take care \(**cleanup**\) of such groups and users, and in order to do it more easily you can use [our Cleanup reports](security-manager-2-release-note.md#internal/get-to-know-security-manager/permissions-reports-screen#cleanup)
* **Compare** SharePoint Online and On-Premises permissions for a selected securable object, as well as track permissions differences using the **Compare Wizard**. The following Compare options are available:
  * Compare permissions with a previous snapshot
  * Compare permissions with a parent

## Bug Fixes

* Fixed error when trying to connect to a site collection via a non-authenticated proxy.
* Fixed error when trying to explore permissions for Office 365 groups site collections that have a special character in their names.

