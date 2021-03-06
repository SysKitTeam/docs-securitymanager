---
title: Global Administrator Consent
description: >-
  This article discusses why global administrator consent is needed for SysKit
  Security Manager
author: Vinko Bedek
date: 09/04/2018
---

# Global Admin Consent

## Why does SysKit Security Manager need consent from a global administrator?

To achieve its functionality, SysKit Security Manager is registered as an Azure Active Directory Application. Azure Active Directory Applications can use other resources from Azure. To use these resources the user running the application must consent to the permissions that the application requires.

When a global administrator uses SysKit Security Manager he will go through the normal consent flow where a popup with the Microsoft consent page is shown. But, when the same action is performed with a non-admin user the action will fail unless administrative consent has been given to the application on the organization level. This is because of the permissions that SysKit Security Manager requires fall in the scope of delegated permissions that need global administrator consent.

## What permissions does SysKit Security Manager require?

SysKit Security Manager requires the following delegated permissions:

* Read all users full profiles
  * Required for reading information about users, ie. the sign-in blocked status
* Read and write all groups
  * Required for Office 365 Groups & Teams functionality
* Read directory data
  * Required for reading additional data from the Azure AD such as directory roles and memberships, ie. checking if the current user is a global admin
* Have full control of all site collections
  * Required for managing SharePoint permissions and assigning site collection administrators
* Read items in all site collections
  * Required to get the SharePoint site url of Office 365 Groups by using the Graph API
* Read all usage reports
  * Required for reading OneDrive and Office 365 Groups activity
* Access Azure Service Management as you
  * This is used to retrieve tenants associated with the account using SysKit Security Manager
* Send mail as a user
  * Required for sending scheduled reports

{% hint style="warning" %}
Granting delegated permissions to an application means that the application may act on behalf of a user. This means that the effective permissions that the user has are still limited by his own permissions. I.e. a user running SysKit Security Manager will not be able to add group owners if he does not have permissions to do so.
{% endhint %}

## Additional Info

* More details on how permissions and consent work in Office 365 can be found in the following [article](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-permissions-and-consent).  
* Click [here](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-applications-guiding-developers-requiring-user-assignment) to learn more on how to limit the consent given to specific users if you choose to do so.

If you at any time decide to revoke the given consent, you can do so by:

1. Go to [Microsoft Azure portal](https://portal.azure.com).
2. Select **Azure Active Directory**.
3. Select **Enterprise Applications**.
4. Select **SysKit Security Manager**.
5. Use the **Delete** button.

