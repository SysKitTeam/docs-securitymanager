---
title: Install SysKit Security Manager
description: >-
  This section describes how to configure, that is install, SysKit Security
  Manager.
author: Petra Filipi
date: 14/03/2018
---

# Install SysKit Security Manager

## Installation Steps

1. [Download](https://www.syskit.com/products/security-manager/download) application.
2. Unpack and run **SysKitSecurityManagerSetup.exe**. The wizard will guide you through the installation steps, click **Next &gt;** to proceed. 
3. Click **I Accept the terms of the license agreement** to accept the license and then click **Next** &gt; to proceed.
4. Select a setup type:  **Default** or **Advanced**. With the default installation type no additional configuration is required.
5. Choose the installation folder e.g. **C:\Program Files\SysKit\Security Manager.** Click **Next** &gt; to proceed.
6. The installation wizard will unpack your files and you will be able to run the application from: **Start** &gt; **All Programs** &gt; **SysKit Security Manager**. 

### Advanced Installation

Installs the **SysKit Security Manager Service** which allows you to take scheduled snapshots while the application is not running. Requires a **dedicated SQL Server database** and a [Service Account](https://github.com/SysKitTeam/docs-securitymanager/tree/7a41ecf00806ae7d8f47809e3c4d6fedecb7bd0c/en-us/windows/security/identity-protection/access-control/service-accounts/README.md). A service account is a user account that is created explicitly to provide a security context for services running on Windows Server operating systems. The security context determined the service’s ability to access local and network resources. The Windows operating systems rely on services to run various features. These services can be configured through the applications, the Services snap-in, or Task Manager, or by using Windows PowerShell.

**SysKit Security Manager Configuration Wizard** will automatically start when you start SysKit Security Manage for the first time. Alternatively, you can start it manually by running it from the installation folder \(default is C:\ProgramFiles\SysKit\Security Manager\Host\SysKit.SecurityManager.ConfigurationWizard.exe\). Follow the steps [here ](../configuration.md)to successfully configure the application.

