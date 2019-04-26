---
description: >-
  This article explains how to configure the SysKit Security Manager database
  and service before the first usage.
---

# Configuration

**SysKit Security Manager Configuration Wizard** will automatically start when you start SysKit Security Manager for the first time. Alternatively, you can start it manually by running it from the installation folder. The default location is:  
'C:\ProgramFiles\SysKit\Security Manager\Host\SysKit.SecurityManager.ConfigurationWizard.exe'.

Follow these steps to successfully configure the application:

{% hint style="info" %} With the **Default** installation type no additional configuration is required and it's suitable for most users. If you want to take scheduled snapshots and reports while the application is not running you should choose the **Advanced** type of installation which requires a dedicated SQL Server database and a service account.
{% endhint %}

1. On the **Welcome** wizard page choose the preferred **setup type**.

   **Default Installation**

   The default installation mode is suitable for most users. Use this option to quickly connect to and manage your site collections and use the basic features. No additional configuration is required.   
   On close, SysKit Security Manager will minimize to the system tray, so you can still use snapshot schedule and schedule reports features while the application is running. Also, you can choose to start SysKit Security Manager on Windows start. You can change this behavior in the[ settings](../get-to-know-security-manager/settings-screen.md#general-settings).

   **Advanced Installation**

   The advanced installation mode is recommended for advanced users. Use this option if you want to collect Office 365 audit logs, take automatic snapshots and receive subscriptions. It will install the **SysKit Security Manager Service** which allows performing background operations and data collection while the application is not running. Requires a **dedicated SQL Server database** and a [Service Account](../requirements/user-permissions-requirements.md#service-account-permissions).

2. On the **Database** wizard page select whether to create a new database or use the existing one. If this is your first time setting up the application choose the **Create new database**. 
3. On the **Database Configuration** wizard page specify the **SQL Server**, **Database Name** and authentication. It is possible to overwrite the existing database under the same name.
   + if you are using the default instance type “servername”, or “servername.yourdomain.loc”
   + if you are using a named instance type “servername\instancename”, or “servername. Yourdomain.loc\instancenameˇ 
   + if your SQL Server is on a non-standard port \(different from 1433\), type “servername,port” or “servername\instance,port”. \(FQDN formats are also supported\)  

    After providing the information, click the **Test Connection** button to ensure that the settings are correct.

4. On the **Service Configuration** wizard page type the service account details. The service account needs to have the [following privileges](requirements/user-permissions-requirements.md#service-account-permissions) to be able to run the service, create snapshots and other associated jobs. After typing the account details, click the **Validate Account** button to ensure that account has all requirements.
5. On the **Security Settings** wizard page you can add a user who can access SysKit Security Manager. Install account is by default on the list. All users with access will be able to see all the data in the application. **Please note** that, while you can add any number of users here, there is no point in doing so as **every user will require a separate license.** 
6. Click **Next** to complete the Configuration Wizard and apply the changes.

