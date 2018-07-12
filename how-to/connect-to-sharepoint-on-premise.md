---  
title: Connect to SharePoint On-Premise Site Collections
author: Petra Filipi 
date: 10/07/2018 
description: This section describes how to connect to a single or multiple SharePoint On-Premise site collections from SysKit Security Manager.
--- 
Choose SharePoint __On-Premise__ to start the connection wizard.

### Credentials
1.	Enter your login name and password. Then click the __Test Credentials__ button and __Next__ to proceed.

### Flow Selection
2.	If you are a __Farm Administrator__, you’ll be able to automatically discover all site collections in a selected farm.
	* Enter __SharePoint Configuration Database__ details. Click __Test Connection__ button and then __Discover__.

	If you are a __Site Collection Administrator__, you can connect to site collections manually.

### Site Collections
3. If you are a __Farm Administrator__, all site collections from your farm will be auto-discovered and you’ll be able to select site collections you want to manage.

    If you are a __Site Collection Administrator__, connect to on-premise site collection by __entering its URL__ or you can __import a text file with site collection URLs__, newline separated. Then, click the __Test Connection__ button and __Next__ to proceed.
	* If you choose the __Import from file__ option, you’ll be able to download the PowerShell script, which will generate a .txt file that you can import. Copy the downloaded script on the SharePoint server, then execute it and then import the file.

### Summary
4. Here is an overview of all the site collections that will be added. You can always edit these from the main navigation.
