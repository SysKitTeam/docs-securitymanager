---
title: Global Administrator Consent
description: This article discusses why global administrator consent is needed for SysKit Security Manager
author: Vinko Bedek
date: 09/04/2018
---

## Why does SysKit Security Manager need consent from a global administrator?

To achieve its functionality, SysKit Security Manager is registered as an Azure Active Directory Application. Azure Active Directory Applications can use other resources from Azure.
To use these resources the user running the application must consent to the permissions that the application requires. 

When a global administrator uses SysKit Security Manager he will go through the normal consent flow where a popup with the Microsoft consent page is shown.
But, when the same action is performed with a non admin user the action will fail unless administrative consent has been given to the application on the organization level.
This is because the permissions that SysKit Security Manager requires fall in the scope of delegated permissions that need global administrator consent.

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
* Access your data anytime
    * Allows refresh token usage, prevents unwanted login prompts on application start
* Read all usage reports
    * Required for reading OneDrive and Office 365 Groups activity
* Access Azure Service Management as you
    * This is used to retrieve tenants associated with the account using SysKit Security Manager

Granting delegated permissions to an application means that the application may act on behalf of a user. 
This means that the effective permissions that the user has are still limited by his own permissions. I.e. a user running SysKit Security Manager will not be able to add group owners if he does not have permissions to do so.

## Additional Info

- More details on how permissions and consent work in Office 365 can be found in the following [article](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-permissions-and-consent).  
- Click [here](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-applications-guiding-developers-requiring-user-assignment) to learn more on how to limit the consent given to specific users if you choose to do so.

If you at any time decide to revoke the given consent, you can do so by:

1. Go to [Microsoft Azure portal](https://portal.azure.com).
2. Select __Azure Active Directory__.
3. Select __Enterprise Applications__.
4. Select __SysKit Security Manager__.
5. Use the __Delete__ button.

