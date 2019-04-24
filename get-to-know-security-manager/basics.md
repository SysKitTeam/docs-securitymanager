---
title: Snapshot Explained
author: Vinko Bedek
date: 03/12/2018
description: This article describes the concept of a snapshot.
---

# Snapshot Explained

## Connecting to an Environment

The application can only be used once connected to an environment. After the first startup, you will be asked to connect to either an[ Office 365](../how-to/connect-to-office-365.md) or your [SharePoint On-Premise](../how-to/connect-to-sharepoint-on-premise.md) environments. In the **Connection Wizard** depending on the permissions of the current user, you will be able to choose the site collections, Office 365 Groups & Teams and OneDrive accounts that you want to connect to. Ordinary site collection administrators will not be able to select from a list of site collections but will need to input them manually.  
There are special considerations to be taken into account when working with a non-global administrator account. Learn more in the [user permission requirements](../requirements/user-permissions-requirements.md) article.

Once connected additional environments can be added by using the Connect button. Connecting to the same environment is also supported when wishing to add additional connected objects. Just select the name of the tenant or On-Premises web application from the Connect button dropdown.

## Snapshot

After connecting your environment to SysKit Security Manager you will undoubtedly come across areas of the application where a snapshot is required.  
A snapshot is nothing more than the collection of all the data needed for SysKit Security Manager to generate reports in a specific point in time. Gathering the data in a single process enables us to provide more complex and faster reports, and to avoid collecting the same data multiple times when jumping from report to report.

Once you have a snapshot created you can view all of the reports available. Creating snapshots will also allow generating permission differences between two points in time.

### Creating a Snapshot

A snapshot can be created from most of SysKit Security Manager. The most prominent location is on the [overview screen](overview-screen.md) after connecting to your environment. The **Take Snapshot** button will always be denoted with a photo camera icon.

### Types of Snapshots

There are two types of Snapshots:

* **Discover & Load Everything** - allows you to create a full snapshot of your environment. SysKit Security Manager will automatically detect and load from new site collections, Office 365 Groups, Microsoft Teams and OneDrive accounts. This may take a while.
* **Custom** **Snapshot** - gives you the ability to manage site collections, Office 365 groups, Microsoft Teams and OneDrive accounts for snapshots. This option will not run the discovery process of your environment. 

