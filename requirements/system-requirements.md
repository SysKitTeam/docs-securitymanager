---
title: System Requirements
description: This article discusses the hardware and software requirements that are necessary in order to install the SysKit Security Manager.
author: Petra Filipi
date: 14/03/2018
---

## Software
* Microsoft Windows 7 (with Service Pack 1), Windows 8, Windows 8.1, Windows 10 or later are supported (64-bit only)
* Microsoft .NET Framework 4.5 or higher

## Hardware
* An Intel or AMD 64-bit CPU that's SSE2 capable
* 512MB of RAM (1GB recommended)
* 1366x768 or higher resolution video card
* 150MB of available hard disk space

## Database System
* SysKit Security Manager Setup will install and configure a new instance of __SQL Server Express 2016 Service Pack 1 LocalDB__ named SSMInstance. 
    * LocalDB instance can be located in the following directory:
_%LOCALAPPDATA%\SysKit\Security Manager\Db_

* By default, access to the instance of LocalDB is limited to its owner.
