---
title: User Permission Requirements
description: >-
  This article discusses the user permission requirements that are necessary in
  order to successfully use SysKit Security Manager.
author: Petra Filipi
date: 14/03/2018
---

# User Permissions Requirements

## Installation

To install SysKit Security Manager, you need to have **Local Administrator** privileges on the target installation computer. Once installed, SysKit Security Manager can be used with a non-privileged user account.

There are two ways of installing SysKit Security Manager in regard to the database install location and the required user account permissions.

### Default Installation

* SysKit Security Manager Setup will install and configure a new instance of **SQL Server 2012 Express LocalDB** named SysKitSecurityManagerInstance.
* **By default, access to the instance of LocalDB is limited to its owner.**
* LocalDB instance can be located in the following directory:

  _%LOCALAPPDATA%\SysKit\Security Manager\Db_

### Advanced Installation

#### Creating a new database

To be able to create a new SysKit Security Manager dedicated database, the **user account running the installation and configuration wizard should have the following rights** on the preferred SQL server:

* **dbcreator**
* **securityadmin**

This allows the account to create a new database and to assign proper privileges after database creation. The install account will be automatically given **db\_owner** privileges on the newly created database, if possible. Otherwise, it is advised that the account is given that privilege manually, as it is needed for upgrading the database.

#### Using the existing database

User running SysKit Security Manager will need to be granted the **db\_datareader** rights on the existing Syskit Security Manager database.

#### Service Account Permissions

**Service Configuration** wizard page requires appropriate [service account](https://docs.microsoft.com/en-us/windows/security/identity-protection/access-control/service-accounts) details.

A service account is a user account that is created explicitly to provide a security context for services running on Windows Server operating systems. The security context determined the service’s ability to access local and network resources. The Windows operating systems rely on services to run various features. These services can be configured through the applications, the Services snap-in, or Task Manager, or by using Windows PowerShell.

**The service account needs to have the following privileges** to be able to run the service, create snapshots and other associated jobs:

* **local administrator** privileges on this computer with UAC control disabled so we can verify your credentials
* **db\_owner** privileges on the created SysKit Security Manager dedicated database
* **log on as Service** rights configured

{% hint style="info" %}
If the service account is outside your domain the account name must be typed in the down-level logon name format: _**domain\accountname**_
{% endhint %}

## Office 365 Permission Requirements

To successfully manage SharePoint permissions, Office 365 Groups, and more, you need to have the following privileges:

### SharePoint Online Permissions

* **Office 365 Global Administrator** Needed to retrieve [Office 365 Audit Logs](../how-to/connect-to-office-365.md#audit-logs) \(**optional**\).
* **Site Collection Administrator** On each site collection you wish to manage.
* **Group Owner** On each group site you wish to manage.
* **OneDrive Site Collection Administrator** On each OneDrive you wish to manage.
* **Azure Active Directory Application Registration** Delegated permissions \([see below](user-permissions-requirements.md#azure-active-directory-application-registration)\).

### Global Administrator Consent

**If the account used to connect to the Office 365 tenant is a global administrator, consent can be given directly from SysKit Security Manager.**

![Global Administrator Consent](../.gitbook/assets/admin-contoso.png)

**Have questions about global admin consent?** Find more information in [**this article**](global-admin-consent.md) or [**contact us!**](https://www.syskit.com/contact-us/)

### Site Collection Administrator

The procedure for using SysKit Security Manager with a Site Collection Administrator account is a bit more involved and will require the global administrator to intervene and [give consent](global-admin-consent.md) on behalf of the users in the organization. While there are permissions that the user itself can consent to, SysKit Security Manager requires some for which only a global administrator can consent.

Once established that the account is a non-global administrator account a window will be shown with a generated URL to give to the global administrator. The consent process can then be initiated by the global administrator.

![Office 365 Global Admin Consent Needed ](../.gitbook/assets/office-365-global-admin-consent-needed.png)

Global administrators considering giving organization wide consent can learn more [here](global-admin-consent.md).

### Azure Active Directory Application Registration

To achieve its functionality, SysKit Security Manager is registered as an **Enterprise Application in Azure Active Directory.** The permissions model is based on OAuth and OpenID Connect flows. This enables us to consume all of the APIs provided by Microsoft in a standard and well defined way. It also enables us to use modern authentication including Multi-Factor Authentication.  
Because of this, when first connecting to an Office 365 tenant the user will be prompted to consent to a set of permissions that SysKit Security Manager requires to function properly. Additional prompts may show up in the future when installing a newer version of SysKit Security Manager because of new functionality and in consequence potentially new required permissions.

For more details on how permissions and consent work in Office 365 you can read the following [article](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-permissions-and-consent). Be warned, it gets a bit technical.

The key takeaway from the article is the concept of effective permissions:

{% hint style="warning" %}
**Please note!**  
The effective permissions of an app will be the least privileged intersection of the delegated permissions the app has been granted \(via consent\) and the privileges of the currently signed-in user. Your app can never have more privileges than the signed-in user.
{% endhint %}

## SharePoint On-Premises Permission Requirements

* **Farm Administrator** For automatic site collection discovery \(**optional**\).
* **Site Collection Administrator** On each site collection you wish to manage.

