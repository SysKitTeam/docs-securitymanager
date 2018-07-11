---  
title: Connect to SharePoint On-Premise Site Collections
author: Petra Filipi 
date: 10/07/2018 
description: This section describes how to connect to a single or multiple SharePoint On-Premise site collections from SysKit Security Manager.
--- 
Choose SharePoint On-Premise to start the connection wizard.
Credentials
1.	Enter your login name and password. Then click the Test Credentials button and Next to proceed.
Flow Selection
2.	If you are a farm administrator you’ll be able to automatically discover all site collections in the selected farm.
a.	Enter SharePoint Configuration Database details. Click Test Connection and then Discover. 
If you are a site collection administrator you can connect to site collections manually.
Site Collections
2.	Connect to on-premise site collection by entering its URL or you can import a text file with site collection URLs, newline separated. Then click the Test Connection button and Next to proceed.
a.	If you choose the Import from file option you’ll be able to download the PowerShell script that will generate a .txt file which you can import. Copy downloaded script on SharePoint server and execute it and then import the file.
3.	If you are a farm admin all site collections from your farm will be auto-discovered and you’ll be able to select site collections you want to manage.
Summary
4.	Here is an overview of all site collections that will be added. You can always edit these from the main navigation.
