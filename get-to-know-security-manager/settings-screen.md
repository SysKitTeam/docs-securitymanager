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
**Start SysKit Security Manager on Windows start** unchecked – use this option if you want to start SysKit Security Manager on Windows start. This option is only available in the default type of installation.  
**On closing, keep the application running**: checked – SysKit Security Manager will close to the system tray.  
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

5. Select the Office 365 credential from the list and click the **Sign in to your Office 365 account again** button.
6. You’ll be redirected to the Microsoft login page and asked to sign in to your account. 

**Delete Credentials**

1. Select the credential from the list and click the **Delete Credentials** button. 
2. If there are no connections for the selected credential click **Delete Credential** to confirm. 

### **About Product**

Here you'll see your **product and database version**.

**Advanced** – If you have the [advanced](../installation/) type of installation, here you can see your service account details, database type, server, database name and if the integrated security is enabled.  
**Participate in Customer Improvement Program** – Here you can choose to participate in the _Customer_ Experience Improvement Program, or unsubscribe from the program at any time.  
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

Here you can enable snapshot schedule, so SysKit Security Manager will [automatically take snapshots](../how-to/scheduled-snapshots.md) of your environment at the time and date you specify. Only one schedule can be active at a time.

You can choose from two types of schedules:

* **Entire Environment** - creates a full snapshot of your environment. New site collections, Office 365 Groups, Teams and OneDrive accounts will automatically be detected and loaded.
* **Custom** - choose which individual site collections, Office 365 Groups, Teams and OneDrive accounts will be in the snapshot. This option will not run the discovery process on your environment. This is a default schedule type.

#### **Date & Time**

By default, the report is scheduled on 8 AM, weekly, recurring on Monday. However, you can adjust it to the time you prefer. You can choose how frequent will the snapshot be performed and depending on the frequency you have selected \(weekly or monthly\), you will also be able to choose on which day will the snapshot be recurring.

## **Audit**

### **Audit Logs**

By enabling the collection of Office 365 audit logs, you can find out about the activities of admins and users within your organization.

{% hint style="warning" %}
**Please note!**  
By enabling Audit Logs in Settings, you enable the collection of Office 365 audit logs for **all connected tenants**.  
In case you want to **enable the audit log collection for a specific tenant only**, enable the Audit Logs option in the Connect Wizard.
{% endhint %}

The information about **Index Size** and the **number of events** in the belonging index is provided here too.

Also, here you can **change the location** where all collected audit logs from your tenant will be stored.

If you want to check and edit which activities are going to be collected, click on the **Select activities to collect** link.

## **Data Retention**

### **Data retention Policy**

With this option, you can **allow Syskit Security Manager to automatically delete old data** from its storage. You can allow the application to remove snapshots and/or audit logs that are older than a certain number of days, weeks or months.

By default, SysKit Security Manager service will execute the Data Retention job every day at a random time between 4:00 AM and 5:00 AM.

If you enable data retention for **Snapshots**, Syskit Security Manager will delete every snapshot from the database that is **older than a specified date**, along with the snapshots you deleted manually in the app.

In case you enable the **Audit Logs** data retention option, audit logs folders **older than a specified date will be deleted**.

For audit logs, you must enter your email address in order to be alerted when Syskit Security Manager notices a certain percentage of disk usage. **A** **warning email will be sent** in case the disk usage is over 85%.

You will also **be alerted via email when Syskit Security Manager stops collecting data** if the disk usage reaches a critical limit of 95%.

