---  
title: SysKit Security Manager Frequently Asked Questions
author: Petra Filipi 
date: 14/03/2018 
description: A list of commonly asked questions.
--- 
This article lists some of the commonly asked questions.

## Can I connect to SharePoint On-Premise site collection?
Yes, SysKit Security Manager works with both SharePoint Online and On-Premise site collections.

## Can I connect to multiple site collections at once? 
If you are a __Global Administrator__ in an Office 365 tenant or a __Farm Administrator__ in a SharePoint On-Premise environment, you will be able to automatically discover and connect to all site collections (including Office 365 Groups) in the tenant or farm.
If you are a __Site Collection Administrator__, you will be able to add multiple connections manually by entering the site collection URLs or by importing a text file with the site collection URLs, newline separated.

## Can I see OneDrive reports without making myself an administrator on user OneDrive accounts?
If you are a Global Office 365 tenant administrator, you’ll have an option in the connection wizard to [connect to all OneDrive accounts](#internal/how-to/connect-to-office-365).

The only way we can access user data and create OneDrive reports is if admin is site collection administrator on user OneDrive accounts. Unfortunately , there is currently no other supported way by Microsoft to do so. Please note that these reports are optional, and if you do not wish to explore them just skip the step in the Connection Wizard. No permissions will be granted to you when it comes to OneDrive sites.

At any time, you can disconnect all OneDrive accounts and remove administrator rights for all OneDrive accounts on the selected tenant using the Disconnect OneDrive action.

## Why am I seeing all the external users on my root site collection?
SysKit Security Manager shows all the external users that have accessed your site collection.
When you share with someone a link to e.g. a Word document, that link will actually point to a document viewer located on the root site collection.
So, when the user navigates to that provided link he will be added to the user list of the root site collection, even though the only content that he can view is located on another site collection.

## Where does SysKit Security Manager store its data?
All of the SysKit Security Manager data is stored __per user__ in the Application Data __%APPDATA%__ directory. SysKit Security Manager uses __Microsoft SQL Server LocalDB__ and stores the database files in the __%LOCALAPPDATA%\SysKit\Security Manager\Db__ folder. To get a fresh start, you can delete the files in this folder. When started, SysKit Security Manager will then create the database files from scratch.
You can also connect to this database by using the following instance name: __\SysKitSecurityManagerInstance__
