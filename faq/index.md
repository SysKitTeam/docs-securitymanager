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

## Why am I seeing all the external users on my root site collection?
SysKit Security Manager shows all the external users that have accessed your site collection.
When you share with someone a link to e.g. a Word document, that link will actually point to a document viewer located on the root site collection.
So, when the user navigates to that provided link he will be added to the user list of the root site collection, even though the only content that he can view is located on another site collection.

