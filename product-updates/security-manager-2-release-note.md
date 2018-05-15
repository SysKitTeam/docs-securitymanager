---
title: SysKit Security Manager 2.0.0 - Release Note
date: 16/05/2018 
description: This article describes what's new and improved in the latest version of SysKit Security Manager.
---
SysKit Security Manager is centralized __SharePoint and Office 365 security reporting and management tool__. It was created to help SharePoint site collection administrators with controlling the security in their SharePoint and Office 365 environment. 

[Try SysKit Security Manager Free](https://www.syskit.com/products/security-manager/download/)

__Product version:__ 2.0.0  
__Build number:__ 599     
__Release date:__ May 16, 2018  

## Features
* __SharePoint Online and On-Premises Snapshots__ are now available in SysKit Security Manager! In addition to being able to manage SharePoint Online and On-Premises permissions, you can now take snapshots of all your site collections and Office 365 groups. This is required in order to use more advanced __Permission Reports__

* Use the __Permissions Reports__ screen to gather valuable information about structure, granted permissions, broken permissions inheritance, and more. We broke them down into four categories. For detailed information on every report see [this article](#internal/get-to-know-security-manager/permissions-reports-screen).

    * __Permissions reports:__ 
    
      Auditing SharePoint permissions can be a complex and time-consuming task. Syskit Security Manager allows administrators to drill down and view all permissions, explore permissions history, and create site and user specific reports.
      
    * __User reports:__
    
       These reports can either give you a __summary__ or a __detailed view__ on the permissions that principal has within a particular site collection. 

    * __Externally Shared:__

      A bundle of reports concerning externally shared content and external users.  
      They will give you information about the content that is shared with external users where you can see what permissions those users have on the content, a list of content shared via anonymous links, and even a list of all unlicensed (external) users on your tenant. 

    * __Cleanup:__

      It is a known thing that SharePoint gets cluttered. Users get disabled, they lose permissions, SharePoint groups lose their members and so on. In all these cases it is recommended to manage (__cleanup__) such groups and users. Explore [our Cleanup reports](#internal/get-to-know-security-manager/permissions-reports-screen#cleanup) and find out what you can do. 


* Compare SharePoint Online and On-Premises permissions for a selected securable object, as well as track permissions differences using the __Compare Wizard__. The following Compare options are available:
    * Compare permissions with a previous snapshot
    * Compare permissions with a parent

## Bug Fixes

* Fixed error when trying to connect to a site collection via a non-authenticated proxy.
* Fixed error when trying to explore permissions for Office 365 groups site collections that have a special character in their names.


