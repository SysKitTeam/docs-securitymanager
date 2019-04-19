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
Please note! These reports are optional, and if you do not wish to explore them just skip the step in the wizard. No permissions will be granted to you when it comes to OneDrive sites.
{% endhint %}

At any time, you can remove access from all connected OneDrive accounts which will also remove administrator rights for all connected OneDrive accounts on the selected tenant using the **Remove Access** action. This action will only remove owner permissions which were granted in the Connection Wizard. You can also remove access to OneDrive accounts one by one.

## Summary

Here is an overview of all the site collections for Office 365 groups and teams and personal OneDrive accounts that will be added. You can always edit these from the main navigation.

