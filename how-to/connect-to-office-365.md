---
description: >-
  This section describes how to connect to a single or multiple SharePoint
  Online site collections, Office 365 groups, teams and OneDrive accounts from
  SysKit Security Manager.
---

# Connect to Office 365

Choose **Office 365** \(Online\) to start the connection wizard:

## Credentials

You’ll be redirected to the Microsoft login page and asked to **Sign in** to your account.

## Site Collections

If you are a **Global Office 365 Tenant Administrator**, all site collections from your tenant will be auto-discovered and you’ll be able to select site collections to which you want to add connections.

If you are a **Site Collection Administrator**, you can connect to a site collection by **entering its URL** or you can **import a text file with the site collection URLs**, newline separated.  
Then click the **Test Connection** button and **Next** to proceed.

## Office 365 Groups and Teams

All Office 365 groups and teams from your tenant will be auto-discovered and you’ll be able to **select the Office 365 groups** you want to manage.

## OneDrive

From SysKit Security Manager version 6, if you are a Global Office 365 tenant administrator or a SharePoint administrator, you will get an option to **Connect to selected OneDrive accounts**.

The user running SysKit Security Manager will be granted site collection administrator rights on personal OneDrive accounts selected in the OneDrive step of the Connection Wizard.

Security Manager keeps track of where you were granted rights so you can easily remove access later. Administrator rights you had before using SysKit Security Manager will not be changed.

Security Manager checks if the current user already has site collection administrator permissions through a SharePoint or a Security Group. When removing access from OneDrive in Security Manager, only directly given permissions are removed.

The only way we can access user data and create OneDrive reports is if admin is granted site collection administrator rights to user OneDrive accounts. Unfortunately, there is currently no other supported way by Microsoft to do so.

{% hint style="warning" %}
**Please note!** These reports are optional, and if you do not wish to explore them just skip the step in the wizard. No permissions will be granted to you when it comes to OneDrive sites.
{% endhint %}

At any time, you can remove access from all connected OneDrive accounts which will also remove administrator rights for all connected OneDrive accounts on the selected tenant using the **Remove Access** action. This action will only remove owner permissions which were granted in the Connection Wizard. You can also remove access to OneDrive accounts one by one.

## Audit Logs

From SysKit Security Manager version 7, if you are a Global Office 365 tenant administrator, you have the option to **enable the collection of Office 365 audit logs**.  
  
When connecting to a new Office 365 tenant, **the audit logs collection will by default be enabled**.  
You can disable it by changing the state of the Audit Logs toggle.  
  
Here, you can also **change the Audit Logs location**. This is the location where SysKit Security Manager will **store all collected Office 365 audit logs**, so **make sure you have enough disk space** when choosing this location.

{% hint style="warning" %}
**Please note!**  
  
**The SysKit Security Manager Service** needs to be up and running to collect Office 365 audit logs. To configure the Service, run the SysKit Security Manager's Configuration Wizard and select the **Advanced mode**. 

**Only the Global Office 365 tenant administrator** has the option to enable the collection of Office 365 audit logs.

Audit logs collection is **not available for on-premises site collections.**
{% endhint %}

To collect Office 365 audit logs, SysKit Security Manager connects to the Office 365 Management Activity API.  
  
Here, the first step is the creation of an **Azure AD Application** on your tenant that has the permissions needed to access the Management Activity API data - for this to happen, SysKit Security Manager needs the **consent of a Global Office 365 tenant administrator.** If you visit you Azure AD Admin Center you can find **SysKit Security Manager Audit Collector** app created in the described step.

The Office 365 Management Activity API aggregates audit logs into **tenant-specific content blobs**, which are classified by the type and source of the logs they contain. Although additional content types are available, SysKit Security Manager currently collects activity data for the following content types:

* **Audit.AzureActiveDirectory**
* **Audit.SharePoint**
* **Audit.General**

To access the content blobs, SysKit Security Manager first needs to create **subscriptions to the content types**. This happens immediately after the Azure AD Application is created.  
  
All of the above actions are done before the Summary step is displayed.  
  
Once the Audit Logs option is enabled, the **Audit Log Collector job** will poll every 15 minutes to discover new content blobs that are available for download. For the Audit Log Collector job to run, **the SysKit Security Manager Service is necessary**. Downloaded blobs are processed and all needed information is saved to a defined storage location on disk.   
After they are processed, the blobs themselves are deleted in order to save disk space.

To find more information about the Office 365 Management APIs used by SysKit Security Manager, follow [this link](https://docs.microsoft.com/en-us/office/office-365-management-api/).

## Summary

Here is an overview of all the site collections for Office 365 groups and teams and personal OneDrive accounts that will be added. You can always edit these from the main navigation.

