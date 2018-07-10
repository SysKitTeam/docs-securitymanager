---
title: User Permission Requirements
description: This article discusses the user permission requirements that are necessary in order to successfully use SysKit Security Manager.
author: Petra Filipi
date: 14/03/2018
---
To install SysKit Security Manager you need to have __Local Administrator__ privilege on the target installation computer.

To successfully manage SharePoint permissions, Office 365 Groups and more, you need to have one of the following privileges:
* __Office 365 Global Administrator__
* __Farm Administrator__
* __Site Collection Administrator__
on the desired Office 365 or SharePoint On-Premises environment.

### SharePoint On-Premises Considerations
* Farm administrators have the possibility to __automatically discover__ all site collections in the selected farm.
* To manage all site collections in a SharePoint farm, instead of adding yourself as a Site Collection Administrator on each Site Collection, you can have __Full Control__ permissions granted in the Web Application Policy.


In order to fully utilize management options of SysKit Security Manager for Office 365 Groups you need to be given [consent by a Global SharePoint Online Administrator](#internal/requirements/global-admin-consent).

