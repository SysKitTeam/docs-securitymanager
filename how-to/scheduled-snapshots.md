---
description: This article describes how to efficiently use scheduled snapshots.
author: Lucija Sopić
date: 21/02/2019
---

# Take Scheduled Snapshots

Scheduled Snapshots are a great way to refresh the data you have in your environment as you can [schedule snapshots](../get-to-know-security-manager/settings-screen.md) to be performed at any date and time you want. For instance, you can schedule a snapshot to be taken before you start working so you have your snapshot ready for use when you need it.

Enabling snapshot schedule allows you to take automatic snapshots at the desired time and frequency, but to use this functionality to its fullest potential some requirements have to be met:

1. Default type installation
   * SysKit Security Manager needs to be running. 
2. Advanced type installation 
   * SysKit Security Manager Service needs to be running.
   * The computer on which SysKit Security Manager is installed needs to be running. 

## Take Scheduled Snapshots

There are two ways to schedule a snapshot:

1. Go directly to the **Settings** screen and click on **Snapshot Schedule** under the Snapshot category.  
2. Go to the **Snapshots screen** and click on the **Snapshot Schedule** button on the top right. That will redirect you to the **Settings** screen.

### Schedule Type

* Choose **Entire Environment** if your environment is constantly changing as this option will discover new site collections, Office 365 Groups, Teams and OneDrives so you have an insight into the state of every newly created object.
* Choose **Custom** if you just want to see the updated state of your previously discovered site collections, Office 365 Groups, Teams and OneDrives.

### Date and Time

* Select the time of day to start the snapshot 
* Choose the frequency \(daily, weekly and monthly\) 
* Choose the recurring date – if you chose the frequency to be weekly then you can select any day of the week, and if the frequency is monthly then than you can choose date of the month on which you want the snapshot to be executed. 

