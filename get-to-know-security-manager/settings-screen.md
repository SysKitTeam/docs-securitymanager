---
title: Settings Screen
description: >-
  On the Settings screen you can customize settings of the SysKit Security
  Manager.
author: Petra Filipi
date: 02/10/2018
---

# Settings Screen

To customize SysKit Security Manager settings, click the **Settings** button located in the left navigation.

## General

### General Settings

On the **Settings** screen the available settings and their default values are:

**Enable Verbose Logging**: unchecked – use this option only for diagnostics purposes or when asked by the support team.

**On close, keep the application running**: checked – SysKit Security Manager will close to the system tray.

**Transport Layer Security protocol**: Default – modify the Transport Layer Security protocol option.

**SQL command timeout\(s\)**: 300 – modify the command timeout for the SQL command.

### Credentials List

Here you'll see a list of all the credentials connected to your connections in SysKit Security Manager.

The **Credentials List** shows you all connected site collections, Office 365 Groups, Microsoft Teams and One Drive accounts. In this article you will see how to edit and remove credentials for SharePoint On-Premise, or sign in to your Office 365 account again from SysKit Security Manager.

**Manage On-Premise Credentials**

1. Select the On-Premise credential from the list and click the **Edit Credentials** button. 
2. **Enter** and confirm **New Password**. 
3. Click **Validate Credential**. 
4. Click **Save**.

   **Sign-in to your Office 365 account again**

5. Select the Office 365 credential from the list and click the Sign in to your Office 365 account again button.
6. You’ll be redirected to the Microsoft login page and asked to sign in to your account. 

**Delete Credentials**

1. Select the credential from the list and click the Delete Credentials button. 
2. If there are no connections for the selected credential click Delete Credential to confirm. 

### **About Product**

Here you'll see your product and database version.

**Advanced** –

**Participate in Customer Improvement Program** –

**License Info** – Here you can figure out how many days are left in trial or subscription, and also [Activate](../activation/) or Deactivate the license.

## **Reporting**

### **Report Throttling**

{% hint style="warning" %}
**Please note!**  
Modifying the report throttling limits can cause significant performance issues!
{% endhint %}

**Site collection threshold**: 50 – modify the maximum number of site collections that will be used to generate data for throttled reports.

**Principals threshold**: 100 – modify the maximum number of principals that will be used to generate data for throttled reports.

**Application row count threshold**: 200,000 – modify the maximum number of rows in reports.

**Export row count threshold**: 500,000 – modify the maximum number of rows in exported reports.

### **Schedule Options**

Here you can enable **Report Schedule** option and customize the time of the day to send scheduled reports.

You can also set up your email settings by choosing one of the options:

**Exchange Online \(My Account\)** – This is the default option for Office 365 administrators. Email containing scheduled reports will be sent via Exchange Online on behalf of the current user.

**Outgoing Email Server** – You can set up existing email server information. Email containing scheduled reports will be sent using the supplied information.

## **Snapshot**

### **Snapshot Schedule**

Here you can enable snapshot schedule, so SysKit Security Manager will automatically take snapshots of your environment at the time and date you specify. Only one schedule can be active at a time.

You can choose from two types of schedules:

* **Entire Environment** - creates a full snapshot of your environment. New site collections, Office 365 Groups, Teams and OneDrive accounts will automatically be detected and loaded.
* **Custom** - choose which individual site collections, Office 365 Groups, Teams and OneDrive accounts will be in the snapshot. This option will not run the discovery process on your environment. This is a default schedule type.

#### **Date & Time**

By default, the report is scheduled on 8 AM, weekly, recurring on Monday. However you can adjust it to the time you prefer. You can choose how frequent will the snapshot be performed and depending on the frequency you have selected \(weekly or monthly\), you will also be able to choose on which day will the snapshot be recurring.

