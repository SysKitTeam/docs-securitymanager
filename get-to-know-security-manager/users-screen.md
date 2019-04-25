---
title: Users Screen
description: Detailed information about the users in a Tenant.
author: Mia Tomaić
date: 19/04/2019
---

# Users Screen

To start exploring features and reports, navigate to Users &gt; Single User and select snapshot, your tenant and user.

Available management actions for the Single User report are contextually related to the selected objects, which means the user can **select one or multiple report rows and available actions will appear on the top of the grid**. Available actions are related to the user selected in the user filter, at top of the page.

## All Users

### All Users tab

A list of all users on the tenant. On this report, you can see a list of users, their email and login name. You can see whether the user is licensed, if it's external, and if the sign-in for the user is allowed. Clicking on a user will take you to that users' detailed report, that is the Single User report.

### Audit tab

The **Audit** tab on the All Users report will show you recent configuration activities related to **adding, updating** or **deleting** users, which are performed by the global administrators.  
Here you can easily track user administration activities such as, **user license changes** and other configuration settings related to **managing passwords**, **logins**, **devices**, etc. 

## Single User

### Sites tab

On Sites tab of the Single Users report, you will find a list of all the sites where the selected user has **any kind of access**. The sites include classic site collections, Office 365 Group site collections, and OneDrive sites.

**Contextual actions:**

* **Copy Permissions** - Copy permissions and group memberships of the currently selected user to a different one on the selected site collection\(s\). Before performing an action, a user has two checkbox options available:
  * Copy Site Administrator role - if the source principal is the site collection administrator of the selected site\(s\), the target user will be added as the site administrator as well. 
  * Keep existing destination principal\(s\) permissions and group membership - destination principal\(s\) will acquire all permissions and group membership\(s\) from the source principal.

    Please note that the following will not be copied: sharing links, OneDrive access, and Security Groups membership.
* **Remove User** - Remove the selected user from the selected site collection\(s\).

{% hint style="warning" %}
Please note!

* The following will not be copied: sharing links, OneDrive access, and Security Groups membership.
* In order to successfully manage permissions on a certain site collection, the user running the application needs to be a site collection administrator.
{% endhint %}

he following will not be copied: sharing links, OneDrive access, and Security Groups membership.

### Office 365 Groups & Teams tab

On this report, you will find a list of Office 365 Groups & Teams where the selected user is member or owner. Select one or more groups/teams and the available actions will be shown in the Actions menu.

**Contextual actions:**

* **Copy Memberships** - Copy Office 365 group memberships of the currently selected user to destination user\(s\).
* **Remove User** - Remove the user from the selected Office 365 Groups and Teams.

### Audit tab

The **Audit** tab on the Single User report will show you all activities and actions performed by a particular user. This can be useful if you want to track the behavior of your external users, e.g. track their every click and what they’ve looked and modified.

Audited activities include:

* File accessed, shared, modified, deleted, malware detected …
* Folder created, deleted, copied, restored …
* Sharing access invitation, blocked, anonymous links …
* Site collection created, Office 365 group created, Team created …
* Membership changes related to Sites, Office 365 groups, Teams …
* Administrative changes performed on the Office 365 tenant …