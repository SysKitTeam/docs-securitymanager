---
title: Snapshot
description: This article describes the concept of a snapshot
author: Vinko Bedek
date: 03/12/2018
---

# Snapshot

## Connecting to an Environment

The application can only be used once connected to an environment. After the first startup you will be asked to connect to either an Office 365 or your SharePoint On-Premise environments. In the [Connect wizard ](../how-to/connect-to-office-365.md)depending on the permissions of the current user you will be able to choose the site collections, Office 365 Groups & Teams that you want to connect to. Ordinary site collection administators will not be able to select from a list of site collections but will need to input them manually.  
There are special considerations to be taken into account when working with a non global administrator account. Learn more in the [user permission requirements](../requirements/user-permissions-requirements.md) article.

Once connected additional environments can be added by using the Connect button. Connecting to the same environment is also supported when wishing to add additional connected objects. Just select the name of the tenant or On-Premise web application from the Connect button dropdown.

## Snapshot

After connecting your environment to SysKit Security Manager you will undoubtedly come across areas of the application where a snapshot is required.  
A snapshot is nothing more than the collection of all the data needed for SysKit Security Manager to generate reports in a specific point in time. Gathering the data in a single process enables us to provide more complex and faster reports, and to avoid collecting the same data multiple times when jumping from report to report.

Once you have a snapshot created you can view all of the reports available. Creating snapshots will also allow generating permission differences between two points in time.

### Creating a Snapshot

A snapshot can be created from most of SysKit Security Manager. The most prominent location is on the overview screen after connecting to your environment. The Take Snaphot button will always be denoted with a photo camera icon.

## Types of Snapshots

There are two types of Snapshots:

* **Custom** snapshot - gives you the ability to manage site collections for snapshots. This option will not load new site collections, only existing ones. 
* **Automatic Discovery** - allows you to create a full snapshot of your environment. SysKit Security Manager will automatically detect and load from new site collections in SharePoint.

