---  
title: Connect to SharePoint On-Premise Site Collections
author: Petra Filipi 
date: 10/07/2018 
description: This section describes how to connect to a single or multiple SharePoint On-Premise site collections from SysKit Security Manager.
--- 
Choose SharePoint __On-Premise__ to start the connection wizard.

### Credentials
1.	Enter your login name and password. Then click the Test Credentials button and Next to proceed.

### Flow Selection
2.	If you are a __farm administrator__ you’ll be able to __automatically discover__ all site collections in the selected farm.
	* Enter __SharePoint Configuration Database__ details. Click Test Connection and then Discover. 
If you are a __site collection administrator__ you can connect to site collections manually.

### Site Collections
3. If you are a __farm administrator__ all site collections from your farm will be auto-discovered and you’ll be able to __select site collections__ you want to manage.

    If you are a __site collection administrator__, connect to on-premise site collection by __entering its URL__ or you can __import a text file__ with site collection URLs, newline separated. Then click the Test Connection button and Next to proceed.
	* If you choose the Import from file option you’ll be able to __download the PowerShell script__ that will generate a .txt file which you can import. Copy downloaded script on SharePoint server and execute it and then import the file.

### Summary
4.	Here is an overview of all site collections that will be added. You can always edit these from the main navigation.
