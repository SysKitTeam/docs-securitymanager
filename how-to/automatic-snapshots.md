---
description: >-
This article describes how to efficiently use automatic snapshots.
author: Lucija Sopic
date: 21/02/2019
---

Automatic Snapshots are a great way to have a quicker insight in your environment because you can [schedule snapshots](../get-to-know-security-manager/settings-screen.md) to be perfomed at the date and time you want. For instance, you can schedule a snapshot to be done before you start working so you have your snapshot ready for use when you need it instead of waiting for a snapshot to finish. Since snapshots are required for some reports to work, you have fresh data to work with and using snapshots is faster than using **Live** option when generating reports. 

# Take Automatic Snapshots

To schedule a snapshot, you can either go directly to the **Settings** screen and click on **Snapshot Schedule** under Snapshot category or from **Snapshots** screen by clicking on **Snapshot Schedule**, which will redirect you to the **Settings** screen.

There are two types of automatic snapshots you can use: **Entire Environment** and **Custom**.

* Choose **Entire Environment** if your environment is constantly changing because this option will discover new site collections, Office 365 Groups, Teams and OneDrives so you have an insight into the state of newly created objects.
* Choose **Custom** if you just want to see updated state of your previously discovered site collections, Office 365 Groups, Teams and OneDrives.

## Date and Time

You can customize date and time to suit your needs. Default time is set to 8AM weekly, reccuring on Monday. You can adjust it to suit your needs - any time, daily, weekly on any day of the week, or monthly, at any day of the month. 

**Please note!** If you schedule your snapshot to be done at the time your application is not running, and your chosen installation mode is **Default**, the snapshot will not be done. If you want the snapshot to be done at the time your application won't be running, opt for [advanced installation.](../installation/installation-guide.md#advanced-installation)
