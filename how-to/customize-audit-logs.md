---
description: >-
  This article will help you get the most out of the Audit Logs feature
  available in SysKit Security Manager.
---

# Customize Audit Logs Collection

By default, **SysKit Security Manager collects the majority of available activities**, nevertheless, you have the option to select which activities are being collected.

To see all available activities and manage which of them are collected by SysKit Security Manager, navigate to **Settings** &gt; **Audit** &gt; **Audit Logs**, and click the **Select activities to collect** link. A new window opens, giving you the possibility to **select or deselect** **an activity, or an entire activity group,** for collection.

{% hint style="info" %}
**Tip!**

**To save disk space** used by audit logs data, disable the collection of activities that you consider unnecessary.

**Can't find an activity** in the audit reports? Chances are, it is not collected by default. Review your settings and turn on the collection of wanted activities.
{% endhint %}

Here, you can find a list of all audit log activities available in SysKit Security Manager, grouped by activity categories**.** You can select from **more than 200 activities** currently available, with **the list being regularly updated** with new activities. For each of the activities, you can find the following information:

* **Display Name** - activity name visible in SysKit Security Manager
* **Original Name** - original activity name created by Microsoft visible in Audit logs search
* **Description** - short description of every activity
* **Collected** - column showing if the activity is collected by default

## Sharing and access request activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Accepted access request | AccessRequestAccepted | An access request to a site, folder, or document was accepted and the requesting user has been granted access. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Approved access request | AccessRequestApproved | An access request to a site, folder, or document was approved. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created access request | AccessRequestCreated | User requested access to a site, folder, or document they don't have permissions to access. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Denied access request | AccessRequestDenied | An access request to a site, folder, or document was denied. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Denied access request | AccessRequestRejected | An access request to a site, folder, or document was denied. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated access request | AccessRequestUpdated | An access request to an item was updated. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| User added to secure link | AddedToSecureLink | A user was added to the list of entities who can use a secure sharing link. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created an anonymous link | AnonymousLinkCreated | A user created an anonymous link to a resource. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed an anonymous link | AnonymousLinkRemoved | User removed an anonymous link to a resource. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated an anonymous link | AnonymousLinkUpdated | User updated an anonymous link to a resource. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Used an anonymous link | AnonymousLinkUsed | An anonymous user accessed a resource by using an anonymous link. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created a company shareable link | CompanyLinkCreated | User created a company-wide link to a resource. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed a company shareable link | CompanyLinkRemoved | User removed a company-wide link to a resource. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Used a company shareable link | CompanyLinkUsed | User accessed a resource by using a company-wide link. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added permission level to site collection | PermissionLevelAdded | A permission level was added to a site collection. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| User removed from secure link | RemovedFromSecureLink | A user was removed from the list of entities who can use a secure sharing link. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created secure link | SecureLinkCreated | A secure sharing link was created to an item. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted secure link | SecureLinkDeleted | A secure sharing link was deleted. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Used secure link | SecureLinkUsed | A user used a secure link. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Accepted sharing invitation | SharingInvitationAccepted | User \(member or guest\) accepted a sharing invitation and was granted access to a resource. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Blocked sharing invitation | SharingInvitationBlocked | A sharing invitation sent by a user in the organization was blocked. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created sharing invitation | SharingInvitationCreated | A user shared a resource in SharePoint Online or OneDrive for Business with a user who isn't in the organization's directory. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Withdrew sharing invitation | SharingInvitationRevoked | User withdrew a sharing invitation to a resource. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated sharing invitation | SharingInvitationUpdated | An external sharing invitation was updated. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Unshared file, folder, or site | SharingRevoked | User \(member or guest\) unshared a file, folder, or site that was previously shared with another user. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Shared file, folder, or site | SharingSet | User \(member or guest\) shared a file, folder, or site in SharePoint or OneDrive for Business with a user in the organization's directory. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Application administration activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Added app role assignment grant to user | Add app role assignment grant to user | An app role was assigned to a user in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added app role assignment to service principal | Add app role assignment to service principal | An app role was assigned to a service principal in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added application | Add application | A new application was registered in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added delegation entry | Add delegation entry | Authentication permission was created/granted to an application in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added OAuth2PermissionGrant | Add OAuth2PermissionGrant | OAuth2PermissionGrant was created for an application in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added owner to application | Add owner to application | An owner was added to an application in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added owner to policy | Add owner to policy | An owner was added to a policy in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added owner to service principal | Add owner to service principal | An owner was added to a service principal in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added service principal | Add service principal | An application was registered in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added credentials to a service principal | Add service principal credentials | Credentials were added to a service principal in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Consent to application | Consent to application | Admin consent was granted to an enterprise app in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created application password for user | Create application password for user | An application password was created for a user in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted application | Delete application | An application was removed from Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Hard delete application | Hard Delete application | An application was permanently removed from Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed delegation entry | Remove delegation entry | An authentication permission was removed from an application in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed a service principal from the directory | Remove service principal | An application was deleted/unregistered from Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed credentials from a service principal | Remove service principal credentials | Credentials were removed from a service principal in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set delegation entry | Set delegation entry | A authentication permission was updated for an application in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated application | Update application | Configuration options of an application were changed in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated service principal | Update service principal | Properties of a service principal were updated. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated StsRefreshTokenValidFrom Timestamp | Update StsRefreshTokenValidFrom Timestamp | Updated StsRefreshTokenValidFrom Timestamp. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## User administration activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Added device | Add device | A device was registered with Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added registered owner to device | Add registered owner to device | A registered owner was added to a device in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added registered users to device | Add registered users to device | A registered user was added to a device in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added user | Add user | An Office 365 user account was created. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed user license | Change user license | The license assigned to a user was changed. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed user password | Change user password | Administrator changed the password for a user. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted device | Delete device | A device was deleted from Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted user | Delete user | A user was deleted from Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Device no longer compliant | Device no longer compliant | A device is noncompliant with defined device compliance policy settings. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Device no longer managed | Device no longer managed | A device is no longer managed in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Enable strong authentication | Enable Strong Authentication | A strong authentication method was enabled for a user in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Hard deleted user | Hard Delete user | A user was permanently deleted from Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Reset user password | Reset user password | Administrator reset the password for a user. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Restored user | Restore user | A deleted user account was restored. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set property that forces user to change password | Set force change user password | Administrator set the property that forces a user to change their password on next sign in. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set license properties | Set license properties | License properties were set for a user in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set user manager | Set user manager | A user manager was set in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated device | Update device | A device was enabled/disabled in Azure AD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated external secrets | Update external secrets | Secrets for external-facing services were updated. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated user | Update user | Administrator changed one or more properties of a user account. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Directory administration activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Added domain to company | Add domain to company | A domain was added to an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added a partner to the directory | Add partner to company | A partner \(delegated administrator\) was added to an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created company | Create company | An Office 365 organization was created. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created company settings | Create company settings | An Office 365 organization settings were created. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed domain from company | Remove domain from company | A domain was removed from an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed a partner from the directory | Remove partner from company | A partner \(delegated administrator\) was removed from an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set company information | Set Company Information | Company information for an Office 365 organization was updated. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Turned on Azure AD sync | Set DirSyncEnabled flag on company | Set the property that enables a directory for Azure AD Sync. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set domain authentication | Set domain authentication | Changed the domain authentication setting for an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated the federation settings for a domain | Set federation settings on domain | Changed the federation \(external sharing\) settings for an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set password policy | Set password policy | Changed the length and character constraints for user passwords in an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated domain | Update domain | Updated the settings of a domain in an Office 365 organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Verified domain | Verify domain | Verified that an organization is the owner of a domain. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Verified email verified domain | Verify email verified domain | Used email verification to verify that an organization is the owner of a domain. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Azure AD group administration activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Added group | Add group | A group was created. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added member to group | Add member to group | A member was added to a group. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Add owner to group | Add owner to group | An owner was added to a group. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted group | Delete group | A group was deleted. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Hard delete group | Hard Delete group | A group was deleted from the recycle bin. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed member from group | Remove member from group | A member was removed from a group. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed owner from group | Remove owner from group | An owner was removed from a group. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated group | Update group | A property of a group was changed. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Role administration activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Added member to role | Add member to role | Member added to a role in AzureAD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added user to a directory role | Add role member to role | A user was added to an admin role in Office 365. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed member from role | Remove member from role | Member removed from a role in AzureAD. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed user from a directory role | Remove role member from role | A user was removed from an admin role in Office 365. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set company contact information | Set company contact information | Company-level contact preferences for the Office 365 organization were updated. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Site permissions activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Added user or group to SharePoint group | AddedToGroup | User added a member or guest to a SharePoint group. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created group | GroupAdded | A site administrator or owner created a group for a site or performed a task that resulted in a group being created. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted group | GroupRemoved | A user deleted a group from a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated group | GroupUpdated | A site administrator or owner changed the settings of a group for a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Modified permission level on site collection | PermissionLevelModified | A permission level was changed on a site collection. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed permission level from site collection | PermissionLevelRemoved | A permission level was removed from a site collection. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Broke permission level inheritance | PermissionLevelsInheritanceBroken | An item was changed so that it no longer inherits permission levels from its parent. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed user or group from SharePoint group | RemovedFromGroup | User removed a member or guest from a SharePoint group. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed user or group from site collection | RemovedFromSiteCollection | A user or group was removed from a site collection. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Broke sharing inheritance | SharingInheritanceBroken | An item was changed so that it no longer inherits sharing permissions from its parent. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Restored sharing inheritance | SharingInheritanceReset | A change was made so that an item inherits sharing permissions from its parent. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Requested site admin permissions | SiteAdminChangeRequest | User requested to be added as a site collection administrator for a site collection. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added site collection admin | SiteCollectionAdminAdded | Site collection administrator or owner added a person as a site collection administrator for a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed Site Collection Admin | SiteCollectionAdminRemoved | Site collection administrator or owner removed a person as a site collection administrator for a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Modified site permissions | SitePermissionsModified | Site administrator or owner \(or system account\) changed the permission level that is assigned to a group on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Modified 'Members Can Share' setting | WebMembersCanShareModified | The 'Members Can Share' setting was modified on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Modified access request setting | WebRequestAccessModified | The access request settings were modified on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Site administration activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Allowed user to create groups | AllowGroupCreationSet | A site administrator or owner added a permission level to a site that allows a user assigned that permission to create a group for that site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed exempt user agents | CustomizeExemptUsers | A SharePoint or global administrator customized the list of exempt user agents in the SharePoint admin center. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed device access policy | DeviceAccessPolicyChanged | A SharePoint or global administrator changed the unmanaged devices policy for the organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added exempt user agent | ExemptUserAgentSet | A SharePoint or global administrator added a user agent to the list of exempt user agents in the SharePoint admin center. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Set host site | HostSiteSet | A SharePoint or global administrator changed the designated site to host personal or OneDrive for Business sites. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Enabled legacy workflow | LegacyWorkflowEnabledSet | A site administrator or owner added the SharePoint 2013 Workflow Task content type to the site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Enabled RSS feeds | NewsFeedEnabledSet | Site administrator or owner enabled RSS feeds for a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Enabled Office on Demand | OfficeOnDemandSet | Site administrator enabled Office on Demand. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Enabled document preview | PreviewModeEnabledSet | Site administrator enabled document preview for a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created Sent To connection | SendToConnectionAdded | A SharePoint or global administrator created a new 'Send To' connection on the Records management page in the SharePoint admin center. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted Sent To connection | SendToConnectionRemoved | A SharePoint or global administrator deleted a 'Send To' connection on the Records management page in the SharePoint admin center. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed a sharing policy | SharingPolicyChanged | A SharePoint or global administrator changed a SharePoint sharing policy. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created site collection | SiteCollectionCreated | A SharePoint or global administrator created a new site collection, or a user provisioned their OneDrive for Business site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted site | SiteDeleted | Site administrator deleted a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Cancelled site geo move | SiteGeoMoveCancelled | A SharePoint or global administrator successfully canceled a SharePoint or OneDrive site geo move. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Completed site geo move | SiteGeoMoveCompleted | A site geo move that was scheduled by a global administrator was successfully completed. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Scheduled site geo move | SiteGeoMoveScheduled | A SharePoint or global administrator successfully scheduled a SharePoint or OneDrive site geo move. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Renamed site | SiteRenamed | Site administrator or owner renamed a site . | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

### DeviceAccessPolicyChanged

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Removed unified group | Remove-UnifiedGroup | An Office 365 group was removed from a tenant. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Microsoft Teams activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Added bot to team | BotAddedToTeam | A user added a bot to a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed bot from team | BotRemovedFromTeam | A user removed a bot from a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added channel | ChannelAdded | A user added a channel to a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted channel | ChannelDeleted | A user deleted a channel from a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed channel setting | ChannelSettingChanged | A team member changed the name or description of a team channel. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added connector | ConnectorAdded | A user added a connector to a channel. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed connector | ConnectorRemoved | A user removed a connector from a channel. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated connector | ConnectorUpdated | A user modified a connector in a channel. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added members to team | MemberAdded | A team owner added member\(s\) to a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed members from team | MemberRemoved | A team owner removed member\(s\) from a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed role of members in team | MemberRoleChanged | A team owner changed the role of member\(s\) in a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added tab | TabAdded | A user added a tab to a channel. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Removed tab | TabRemoved | A user removed a tab from a channel. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated tab | TabUpdated | A user modified a tab in a channel. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created team | TeamCreated | A user created a new team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted team | TeamDeleted | A team owner deleted a team. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed team setting | TeamSettingChanged | A team owner changed the name or description of a team, team's access type or information classification, or any of the team settings. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| User signed in to Teams | TeamsSessionStarted | A user signed in to a Microsoft Teams client. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/unchecked.png) |
| Changed organization setting | TeamsTenantSettingChanged | A global admin changed organization-wide Microsoft Teams settings. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

### TeamsTenantSettingChanged

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Changed Conferencing Policy | Grant-CsConferencingPolicy | An administrator assigned a Teams conferencing policy at the per-user scope. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Meeting Broadcast Policy | Grant-CsTeamsMeetingBroadcastPolicy | An administrator assigned a Teams meeting broadcast policy at the per-user scope. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Meeting Policy | Grant-CsteamsmeetingPolicy | An administrator assigned a Teams meeting policy at the per-user scope. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Granted Messaging Policy | Grant-CsTeamsMessagingPolicy | An administrator assigned a Teams messaging policy at the per-user scope. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Upgrade Policy | Grant-CsTeamsUpgradePolicy | An administrator applied a Teams upgrade policy to a user or the entire organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added Meeting Broadcast Policy | New-CsTeamsMeetingBroadcastPolicy | An administrator created a new Teams meeting broadcast policy. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added Meeting Policy | New-CsTeamsMeetingPolicy | An administrator created a new Teams meeting policy. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Added Messaging Policy | New-CsTeamsMessagingPolicy | An administrator created a new Teams messaging policy. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Client Configuration | Set-CsTeamsClientConfiguration | An administrator changed the settings accessed via Teams clients across the organization. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Guest Calling Configuration | Set-CsTeamsGuestCallingConfiguration | An administrator changed which options guest users have for calling within Teams. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Guest Meeting Configuration | Set-CsTeamsGuestMeetingConfiguration | An administrator changed which meeting features guests leveraging Microsoft Teams will have available. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Guest Messaging Configuration | Set-CsTeamsGuestMessagingConfiguration | An administrator changed the messaging settings for guest users. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Meeting Configuration | Set-CsTeamsMeetingConfiguration | An administrator updated a Teams meeting configuration. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Messaging Policy | Set-CsTeamsMessagingPolicy | An administrator updated a Teams messaging policy. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Upgrade Configuration | Set-CsTeamsUpgradeConfiguration | An administrator changed the Teams upgrade configuration. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Changed Federation Configuration | Set-CsTenantFederationConfiguration | An administrator changed federation configuration settings for a Skype for Business Online tenant. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## File and page activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Accessed file | FileAccessed | User or system account accessed a file. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Accessed file extended | FileAccessedExtended | User or system account accessed a file. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Checked in file | FileCheckedIn | User checked in a document that they checked out from a document library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Checked out file | FileCheckedOut | User checked out a document located in a document library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Discarded file checkout | FileCheckOutDiscarded | User discarded changes made to a checked out file. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Copied file | FileCopied | User copied a document from a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted file | FileDeleted | User deleted a document from a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted file from recycle bin | FileDeletedFirstStageRecycleBin | User deleted a file from the recycle bin of a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted file from second-stage recycle bin | FileDeletedSecondStageRecycleBin | User deleted a file from the second-stage recycle bin of a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Downloaded file | FileDownloaded | User downloaded a document from a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Detected malware in file | FileMalwareDetected | SharePoint anti-virus engine detected malware in a file. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Modified file | FileModified | User or system account modified the content or the properties of a document located on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Modified file extended | FileModifiedExtended | User or system account modified the content or the properties of a document located on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Moved file | FileMoved | A user moved a document from its current location on a site to a new location. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Preview file | FilePreviewed | User previewed a document on a SharePoint or OneDrive for Business site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Renamed file | FileRenamed | User renamed a document on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Restored file | FileRestored | User restored a document from the recycle bin of a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Uploaded file | FileUploaded | User uploaded a document to a folder on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Recycled version of file | FileVersionRecycled | User deleted a version from the version history of a file. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Recycled all minor versions of file | FileVersionsAllMinorsRecycled | User deleted all minor versions from the version history of a file. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Recycled all versions of file | FileVersionsAllRecycled | User deleted all versions from the version history of a file. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Viewed page | PageViewed | A user viewed a page on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Viewed page extended | PageViewedExtended | A user viewed a page on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Search query performed | SearchQueryPerformed | User performed a search query on a SharePoint or OneDrive for Business site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Synchronization activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Downloaded files to computer | FileSyncDownloadedFull | User successfully downloaded files for the first time to their computer from a document library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Downloaded file changes to computer | FileSyncDownloadedPartial | User successfully downloaded changes to files from a document library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Uploaded files to document library | FileSyncUploadedFull | User successfully uploaded files for the first time from their computer to a document library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Uploaded file changes to document library | FileSyncUploadedPartial | User successfully uploaded changes to files on a document library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Allowed computer to sync files | ManagedSyncClientAllowed | User successfully established a sync relationship with a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Blocked computer from syncing files | UnmanagedSyncClientBlocked | User's computer was blocked from syncing, downloading, or uploading files on a document library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Folder activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Copied folder | FolderCopied | User copied a folder from a site to another location in SharePoint or OneDrive for Business. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created folder | FolderCreated | User created a folder on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted folder | FolderDeleted | User deleted a folder from a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted folder from recycle bin | FolderDeletedFirstStageRecycleBin | User deleted a folder from the recycle bin on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted folder from second-stage recycle bin | FolderDeletedSecondStageRecycleBin | User deleted a folder from the second-stage recycle bin on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Modified folder | FolderModified | A user modified a folder on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Moved folder | FolderMoved | A user moved a folder to a different location on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Renamed folder | FolderRenamed | User renamed a folder on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Restored folder | FolderRestored | User restored a deleted folder from the recycle bin on a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## Data governance

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| List column created | ListColumnCreated | A column was created in a SharePoint list or library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| List column deleted | ListColumnDeleted | A column was deleted from a SharePoint list or library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| List column updated | ListColumnUpdated | A column was updated in a SharePoint list or library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| List content type created | ListContentTypeCreated | A content type was created in a SharePoint list or library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| List content type deleted | ListContentTypeDeleted | A content type was deleted from a SharePoint list or library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| List content type updated | ListContentTypeUpdated | A content type was updated in a SharePoint list or library. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Site column created | SiteColumnCreated | A column was created in a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Site column deleted | SiteColumnDeleted | A column was deleted from a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Site column updated | SiteColumnUpdated | A column was updated in a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Site content type created | SiteContentTypeCreated | A content type was created in a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Site content type deleted | SiteContentTypeDeleted | A content type was deleted from a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Site content type updated | SiteContentTypeUpdated | A content type was updated in a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## SharePoint list events

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| Created list | ListCreated | A user created a list on a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted list | ListDeleted | A user deleted a list from a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Created list item | ListItemCreated | A user created a list item on a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Deleted list item | ListItemDeleted | A user deleted a list item from a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Recycled list item | ListItemRecycled | A user moved a list item to the recycle bin of a site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated list item | ListItemUpdated | A user updated a list item on a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| Updated list | ListUpdated | A user updated a list on a SharePoint site. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

## User activities

| Display Name | Original Name | Description | Collected |
| :--- | :--- | :--- | :---: |
| User logged in | UserLoggedIn | A user logged into Office 365. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |
| User login failed | UserLoginFailed | Office 365 user login failed. | ![](https://github.com/SysKitTeam/docs-securitymanager/tree/e9daa8942681c16e534975fcac7c570b13b0d260/.gitbook/assets/checked.png) |

