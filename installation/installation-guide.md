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
4. Choose a setup type:  **Default** or **Advanced**. 
5. Choose the installation folder e.g. **C:\Program Files\SysKit\Security Manager.** Click **Next** &gt; to proceed.
6. The installation wizard will unpack your files and you will be able to run the application from: **Start** &gt; **All Programs** &gt; **SysKit Security Manager**. 

## Setup Type

{% hint style="info" %}
With the **Default** installation type no additional configuration is required and it's suitable for most users. If you want to take scheduled snapshots and reports while the application is not running you should choose the **Advanced** type of installation which requires a dedicated SQL Server database and a service account. 
{% endhint %}

### Default Installation

Default installation mode, suitable for most users. No additional configuration is required. On close, SysKit Security Manager will minimize to the system tray, so you can still use snapshot schedule and schedule reports features while the application is running. Also, you can choose to start SysKit Security Manager on Windows start. You can change this behavior in the[ settings](../get-to-know-security-manager/settings-screen.md#general-settings). 

### Advanced Installation

This is the advanced installation mode,  recommended for advanced users. Installs the **SysKit Security Manager Service** which allows you to take scheduled snapshots while the application is not running. Requires a **dedicated SQL Server database** and a [Service Account](../requirements/user-permissions-requirements.md#service-account-permissions). 

**SysKit Security Manager Configuration Wizard** will automatically start when you start SysKit Security Manager for the first time. Alternatively, you can start it manually by running it from the installation folder \(default is C:\ProgramFiles\SysKit\Security Manager\Host\SysKit.SecurityManager.ConfigurationWizard.exe\). Follow the steps [here ](../configuration.md)to successfully configure the application.

