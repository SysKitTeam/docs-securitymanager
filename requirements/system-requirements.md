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
* 300MB of available hard disk space

## Database

In order to run the SysKit Security Manager, you need a database. The SysKit Security Manager supports **SQL Server databases only**.

### Default mode

If you **do not have an SQL Server instance** installed in your environment, the SysKit Security Manager will install the **SQL Server Express 2012 LocalDB** \(free license\) which you can select to use.

### Advanced mode

You can use the following **SQL Server** versions: **SQL Server 2012 – 2017**, all editions. We advise you to use the latest available SQL Server version and apply all the available Service Packs before installing SysKit Security Manager.  
If you are moving your existing LocalDB database to a new SQL server, please follow the instructions in [this article](../how-to/move-localdb-to-new-server.md).

