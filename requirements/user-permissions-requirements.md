---
title: User Permission Requirements
description: >-
  This article discusses the user permission requirements that are necessary in
  order to successfully use SysKit Security Manager.
author: Petra Filipi
date: 14/03/2018
---

# user-permissions-requirements

To install SysKit Security Manager, you need to have **Local Administrator** privileges on the target installation computer.

To successfully manage SharePoint permissions, Office 365 Groups, and more, you need to have one of the following privileges on the desired Office 365 or SharePoint On-Premises environment:

* **Office 365 Global Administrator**
* **Farm Administrator**
* **Site Collection Administrator**

## SharePoint On-Premises Considerations

* Farm administrators have the possibility to **automatically discover** all site collections in a selected farm.
* To manage all site collections in a SharePoint farm, instead of adding yourself as a **Site Collection Administrator** on each site collection, you can have **Full Control** permissions granted in the Web Application Policy.

In order to fully utilize the management options in SysKit Security Manager, you need to be given [consent by a Global SharePoint Online Administrator](user-permissions-requirements.md#internal/requirements/global-admin-consent).

