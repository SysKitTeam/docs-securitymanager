---
description: >-
  This article explains how to configure the SysKit Security Manager database
  and service before the first usage.
---

# Configuration

**SysKit Security Manager Configuration Wizard** will automatically start when you start SysKit Security Manager for the first time. Alternatively, you can start it manually by running it from the installation folder \(default is C:\ProgramFiles\SysKit\SecurityManager\Host\SysKit.SecurityManager. ConfigurationWizard.exe\). Follow these steps to successfully configure the application: 

1. On the **Database** wizard page select whether to create a new database or use the existing one. If this is your first time setting up the application choose the **Create new database**. 

{% hint style="warning" %}
Please note! This should be a SysKit Security Manager-dedicated database; please do not provide SharePoint Database here.
{% endhint %}

2. On the **Database Configuration** wizard page specify the **SQL Server**, **Database Name** and authentication. It is possible to overwrite the existing database under the same name.  

* if you are using the default instance type “servername”, or “servername.yourdomain.loc” 
* if you are using a named instance type “servername\instancename”, or “servername. Yourdomain.loc\instancenameˇ 
* if your SQL Server is on a non-standard port \(different from 1433\), type “servername,port” or “servername\instance,port”. \(FQDN formats are also supported\)  

After providing the information, click the **Test Connection** button to ensure that the settings are correct.  

3. On the **Service Configuration** wizard page type the service account details. The service account needs to have the \[following privileges\]\(link\) to be able to run the service, create snapshots and other associated jobs. After type the account details, click the **Validate Account** button to ensure that account has all requirements.  

4. On the **Security Settings** wizard page you can add user who can access SysKit Security Manager. Install account is by default on the list. All users with access will be able to see all the data in the application.  

5. Click **Next** to complete the Configuration Wizard and apply the changes.





