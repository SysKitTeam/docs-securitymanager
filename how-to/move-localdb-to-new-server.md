---
title: Move LocalDB database to new SQL server
description: >-
  This article describes how to move the LocalDB database that was configured with SysKit Security Manager to a new SQL server.
author: Andrea Budisa
date: 25/04/2019
---

If you are using **Microsoft SQL Server 2012 Express LocalDB** as a database backend with SysKit Security Manager and want to use the **Advanced** configuration option which includes **Office 365 Audit Logs** feature, do not worry, you can still migrate your old data in just a few easy steps.

Please follow these steps to move a LocalDB database to another location:

1. Turn off the SysKit Security Manager application.
2. Navigate to the following location **C:\Users\user_name\AppData\Local\SysKit\Security Manager\Db**. The **'user_name'** is just a placeholder which you need to replace with the user account that was used for the initial configuration process. 
3. Check whether you have all the necessary files in place: **SysKitSMDatabase.mdf** and **SysKitSMDatabase_log.ldf**.  
4. Connect to the SQL server and open the **SQL Management Studio**.
5. Right-click the Databases section and select the **Attach... option**.
6. In the Attach Databases dialog, click the **Add...** button and locate the SysKit Security Manager database, then select **SysKitSMDatabase.mdf** file.  
Note: If you are connecting to a remote SQL server instance, copy the files to the new SQL server.
7. Attach the database by clicking the **OK** button.
8. If the attach is successful, start the **SysKit Security Manager Configuration Wizard** on the computer where the SysKit Security Manager is installed.
9. In the Welcome step, select the **Advanced** configuration option.
10. In the Database step select the **Use existing database** option and in the next step enter the new SQL server and the old database name.
11. In the Service Settings step, type in the service user that has permissions to the database.
12. Go through all the steps until the configuration process is finished.