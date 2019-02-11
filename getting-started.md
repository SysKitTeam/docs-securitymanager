---
description: >-
  Described some of the common use cases when starting the application for the
  first time.
---

# Quick Start Guide

In this article we will take you through some of the common use cases and usual steps when using the application for the first time. We have provided you with an overview of the entire application and how to use it. For detailed information on particular features, please explore our other articles.

## Getting Started

After successfully activating the application, or starting the trial, you will be able to connect to [SharePoint Online](how-to/connect-to-office-365.md) or [On-Premise](how-to/connect-to-sharepoint-on-premise.md) site collection using your Office 365 or SharePoint admin credentials.

After successfully [activating](activation/) the application, or starting the trial, you will be able to [connect to Office 365 ](how-to/connect-to-office-365.md)\([SharePoint Online](how-to/connect-to-office-365.md#site-collections), [Office 365 Groups](how-to/connect-to-office-365.md#office-365-groups-and-teams), [Microsoft Teams](how-to/connect-to-office-365.md#office-365-groups-and-teams), [OneDrive](how-to/connect-to-office-365.md#onedrive)\) or [On-Premise](how-to/connect-to-sharepoint-on-premise.md) site collections using your credentials. After you pick which Site Collections, Groups, Teams and OneDrive accounts you want to manage, the initial snapshot will be triggered. For more details about snapshots, [see this article.](https://github.com/SysKitTeam/docs-securitymanager/tree/4881261de3f4b23178a29ad38c5dcf1c343d8964/basics.md#snapshot)

To successfully manage SharePoint permissions, Office 365 Groups, Microsoft Teams, OneDrive and more, you need to have **one of the following privileges** on the desired Office 365 or SharePoint On-Premises environment:

* **Office 365 Global Administrator**
* **Farm Administrator**
* **Site Collection Administrator**

{% hint style="warning" %}
Please note! **You don't have to be an Office 365 Global Administrator** in order to use SysKit Security Manager, but in order for a regular user to use Security Manager, the administrator must first sign in and consent to permission on behalf of the organisation. This is because the permissions that SysKit Security Manager requires fall in the scope of delegated permissions that need [global administrator consent](requirements/global-admin-consent.md).
{% endhint %}

Afterwards, on the **Site Collections** screen, you can see the site structure and explore and manage the permissions of the site collections you connected. On the **Office 365 Groups** screen, you can see an overview of all connected Office 365 Groups: their settings, owners and members.

For detailed information on user permission requirements, [see this article.](https://github.com/SysKitTeam/docs-securitymanager/tree/4881261de3f4b23178a29ad38c5dcf1c343d8964/user-permissions-requirements.md)

## SharePoint Explorer

The moment you connect to a new site collection, you can explore and manage SharePoint permissions from SysKit Security Manager. SysKit Security Manager works with both SharePoint Online and On-Premise site collections. If you connect to Office 365 Groups, you can see Office 365 Groups site collections.

## Office 365 Groups

The Office 365 Groups screen gives you an overview of Office 365 Groups: their settings, owners and members.

## Microsoft Teams

The Microsoft Teams screen gives you an overview of Microsoft Teams: their settings, owners, and members.

## OneDrive

The OneDrive screen gives you a general overview of your connected personal OneDrive accounts, as well as a report for each OneDrive account.

