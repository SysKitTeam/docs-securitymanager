---
description: >-
This article describes how to efficiently use automatic snapshots.
author: Lucija Sopic
date: 21/02/2019
---

Automatic Snapshots are a great way to refresh the data you have of your environment as you can [schedule snapshots](../get-to-know-security-manager/settings-screen.md) to be performed at the date and time you want. For instance, you can schedule a snapshot to be done before you start working so you have your snapshot ready for use when you need it. 

{% hint style="warning" %}
**Please note!**  
For the scheduled snapshot to work, while installing the application opt for the [advanced installation](../installation/installation-guide.md#advanced-installation) and NOT the **Default** mode. 
{% endhint %}

# Take Automatic Snapshots

There are two ways to schedule a snapshot:
1. You can either go directly to the **Settings** screen and click on **Snapshot Schedule** under Snapshot category.
2. or go to the **Snapshots screen** and click on the **Snapshot Schedule** button on the top right. That will redirect you to the **Settings** screen.

There are two types of automatic snapshots you can use: **Entire Environment** and **Custom**.

* Choose **Entire Environment** if your environment is constantly changing as this option will discover new site collections, Office 365 Groups, Teams and OneDrives so you have an insight into the state of every new created objects.
* Choose **Custom** if you just want to see updated state of your previously discovered site collections, Office 365 Groups, Teams and OneDrives.

## Date and Time

You can customize date and time to suit your needs. Default time is set to 8AM weekly, recurring on Monday. Available frequency is weekly, daily or monthly.


