---
title: Move LocalDB database to a new SQL server
description: >-
  This article describes how to move the LocalDB database that was configured with SysKit Security Manager to a new SQL server.
author: Andrea Budisa
date: 25/04/2019
---

If you are using **Microsoft SQL Server 2012 Express LocalDB** as a database backend with SysKit Security Manager and want to use the **Advanced** configuration option which includes the **Office 365 Audit Logs** feature, do not worry, you can still migrate your old data in just a few easy steps.

Please follow these steps to move a LocalDB database to another location:

1. Turn off the SysKit Security Manager application.
2. Navigate to the following location **C:\Users\user_name\AppData\Local\SysKit\Security Manager\Db**. The **'user_name'** is just a placeholder which you need to replace with the user account that was used for the initial configuration process. 
3. Check whether you have all the necessary files in place: **SysKitSMDatabase.mdf** and **SysKitSMDatabase_log.ldf**.
4. Copy the entire **Db folder** which contains these two files to the **SQL Server Data path**. Location path can vary depending on the SQL Server edition and version, e.g. **C:\Program Files\Microsoft SQL Server\MSSQL14.SQLEXPRESS\MSSQL\DATA**.   
5. After the files are successfully transferred, run the **SQL Management Studio** with elevated privileges and connect to the new SQL server.
6. Right-click the Databases section and select the **Attach...** option.
7. In the Attach Databases dialog, click the **Add...** button and locate the SysKit Security Manager database, then select the **SysKitSMDatabase.mdf** file.  
8. Attach the database by clicking the **OK** button.
9. If the attach is successful, start the **SysKit Security Manager Configuration Wizard** on the computer where the SysKit Security Manager is installed.
10. In the Welcome step, select the **Advanced** configuration option.
11. In the Database step select the **Use existing database** option and in the next step enter the new SQL server and the old database name.
12. In the Service Settings step, type in the service user that has permissions to the database.
13. Go through all the steps until the configuration process is finished.