---
title: System Requirements
description: >-
  This article discusses the hardware and software requirements that are
  necessary in order to install the SysKit Security Manager.
author: Petra Filipi
date: 14/03/2018
---

# System Requirements

## Software

* Microsoft Windows 7 \(with Service Pack 1\), Windows 8, Windows 8.1, Windows 10 or later are supported \(64-bit only\)
* Microsoft .NET Framework 4.5 or higher

## Hardware

* An Intel or AMD 64-bit CPU that's SSE2 capable
* 512MB of RAM \(1GB recommended\)
* 1366x768 or higher resolution video card
* 150MB of available hard disk space

## Database System

### **Default Installation**

* SysKit Security Manager Setup will install and configure a new instance of **SQL Server 2012 Express LocalDB** named SysKitSecurityManagerInstance.
  * LocalDB instance can be located in the following directory:

    _%LOCALAPPDATA%\SysKit\Security Manager\Db_
* By default, access to the instance of LocalDB is limited to its owner.

### **Advanced Installation**

#### **Creating a new database**

 To be able to create a new SysKit Security Manager dedicated database, the user account running the installation and configuration wizard \(i.e. install account\) should be granted both the **dbcreator** and **securityadmin** roles on the preferred SQL Server. This allows the account to create a new database and to assign proper privileges after creation. The install account will be automatically given **db\_owner** privileges on the newly created database, if possible. Otherwise, it is advised that the account is given that privilege manually, as it is needed for upgrading the database. 

#### Using the existing database

 User running SysKit Security Manager will need to be granted the **db\_datareader** rights on the existing Syskit Security Manager database.  

