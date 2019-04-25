---
title: OneDrive Screen
description: >-
  The OneDrive screen gives you a general overview of your connected OneDrive
  accounts.
author: Tomislav Sirovec
date: 23/04/2019
---

# OneDrive

To start exploring features and reports, navigate to the OneDrive screen and select your tenant.

Some actions are globally related to all OneDrive accounts and other are contextually related to the selected object\(s\). Which means that users can select items from the grid by clicking the checkboxes on the left, and perform the desired action\(s\) from the **Actions Toolbar**, such as removing access from OneDrive or stop sharing all documents.

## OneDrive Overview

### OneDrive Overview tab

Gives a general overview of the OneDrive accounts which you've chosen to load. On this report, you can see a list of users, their corresponding OneDrive URLs, different levels of storage usage, as well as check if there was any activity in the last three months.

**Contextual actions:**

* **Remove Access** – This action will remove permissions which were granted in the [connection wizard](../how-to/connect-to-office-365.md#onedrive). 
* **Stop Sharing** – This action will remove all unique permissions from the selected OneDrive. This will disable all anonymous links as well.

### Audit tab

The **Audit** tab on the OneDrive Overview report will show you events related to the **OneDrive creation**, **deletion** and **security changes**, or events which can pose a security issue, e.g. if a global administrator has added and then removed his account from owners on a particular OneDrive, to access data.  
Here you can easily identify if there are any **synchronization issues** between the computers in your organization's domain and OneDrive for Business and get information on whether a user has successfully established a sync relationship with a site.

Audited activities include:

* Site collection created, deleted
* Added site collection admin, removed
* Allowed computer to sync files, blocked 

## Single User's OneDrive

### Single User's OneDrive tab

On the Single User's OneDrive report, you will find a list of all the items in someones OneDrive. You can see who created the item and when, who modified it and when, its file size, and of course whether the item is shared with someone or is it private.

**Global actions:**

* **Remove Access** – This action will remove permissions which were granted in the [connection wizard](../how-to/connect-to-office-365.md#onedrive). 
* **Stop Sharing** – This action will remove all unique permissions from the selected OneDrive. This will disable all anonymous links as well.

### Audit tab

The **Audit** tab on the Single User’s OneDrive report will show you recent activity for the selected OneDrive. The report will show you all the details such as, **file accesses**, **edits** and **modifications**, **sharing activities** \(both external and internal\) for documents or folders in the selected date range.  
Here you can check whether a user has shared files with external users and all the important details like when, with whom, and which file was shared.  
If your users are having issues with the OneDrive sync client, here you can easily check if there has been a **successful upload** or **download** of any changes to files within the selected date range.

Audited activities include:

* File accessed, shared, modified, deleted, malware detected …
* Folder created, deleted, copied, restored …
* Sharing access invitation, blocked, anonymous links …

## OneDrive Reports

* **Orphaned OneDrive** – Shows a list of OneDrive accounts whose owner is disabled or deleted from the Azure Active Directory. Supports live and snapshot data.
* **OneDrive With Guests** – Shows personal OneDrive accounts that have guests or external users with existing permissions.
* **OneDrive Shared Items** – Shows OneDrive items that have been shared. Report can show shared items across multiple OneDrive storages at the same time. For detailed information about permissions on specific shared files this report has built-in drill functionality to Permissions Matrix report.