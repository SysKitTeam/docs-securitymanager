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
Here you can easily track Azure AD user and role administration activities performed in your Office 365 environment, which include **changing user license, setting license properties, adding or removing users from an admin role, adding or removing delegated administrators**.

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
**Please note!**  
The following will not be copied: sharing links, OneDrive access, and Security Groups membership.  
In order to successfully manage permissions on a certain site collection, the user running the application needs to be a site collection administrator.
{% endhint %}

### Office 365 Groups & Teams tab

On this report, you will find a list of Office 365 Groups & Teams where the selected user is member or owner. Select one or more groups/teams and the available actions will be shown in the Actions menu.

**Contextual actions:**

* **Copy Memberships** - Copy Office 365 group memberships of the currently selected user to destination user\(s\).
* **Remove User** - Remove the user from the selected Office 365 Groups and Teams.

### Audit tab

The **Audit** tab on the Single User report will show you all activities and actions performed by a particular user. This can be useful if you want to track the behavior of your external users, e.g. track their every click and what they’ve looked and modified.  
Here you can easily track Azure AD user administration activities such as, **user license changes** and other configuration settings related to **managing passwords**, **logins**, **devices**, etc.

Audited activities include:

* File accessed, shared, modified, deleted, malware detected …
* Folder created, deleted, copied, restored …
* Sharing access invitation, blocked, anonymous links …
* Site collection created, Office 365 group created, Team created …
* Membership changes related to Sites, Office 365 groups, Teams …

## User Reports

* **User Permissions Overview** – A summary of principals' permissions on the tenant. Shows site collections in which users have permissions, permissions that the users have as an individual, and the permissions that were given through a group. 
* **User Permissions Details** – Shows all permissions on all subsites inside a selected site collection for a specific user. The report shows permissions that a certain user has on each item within the particular site collection, along with the permissions that were given through a group. This report can show every object in your environment to which a specified user or users have access to. This includes all SharePoint objects, Groups and Teams objects and OneDrive files.  
* **Users with Privileged Access** – Shows all users with privileged access on the tenant or farm, such as farm and site administrators, or primary and secondary administrators, Users with Full Control / Full Read Web Application Policy, etc. Supports live and snapshot data.
* **Multi-Factor Authentication for Admins** – This report shows which site collection admins have multi-factor authentication enabled. It is recommended that all users with privileged access have Multi-Factor Authentication enabled. [Possible MFA states are](https://social.msdn.microsoft.com/Forums/azure/en-US/46d1e71e-f98a-4e97-94f8-11621c3385d8/mfa-status-enabled-enforced?forum=windowsazureactiveauthentication):
  * **Disabled** - This is the default state for a new user not enrolled in multi-factor authentication.
  * **Enabled** - The user has been enrolled in multi-factor authentication, but has not completed the registration process. They will be prompted to complete the process the next time they sign in.
  * **Enforced** - The user may or may not have completed registration. If they have completed the registration process then they are using multi-factor authentication. Otherwise, the user will be prompted to complete the process at next sign-in. In non-browser apps \(such as Outlook etc.\) will not work until app passwords are created and entered into the non-browser apps.

    In order to use this report the following prerequisites need to be satisfied:

  * PowerShell version 3.0. or newer
  * Latest MSOnline PowerShell module installed - can be installed by running the following powershell commandlet: Install-Module MSOnline