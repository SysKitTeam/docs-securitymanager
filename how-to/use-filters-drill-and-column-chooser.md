---
description: >-
  This article describes how to use Filters, Drill and Column Chooser on your
  reports.
---

# Use Filters, Drill and Column Chooser

## Filters

Before you can view the report data you will need to configure the report filters. The available filters will depend on the selected report. All reports will have at least the Snapshot filter and the SharePoint Objects filter available.

* **Snapshot** - The Snapshot Filter allows you to view the report for a specific snapshot that you have taken. It also contains the Live entry, which can be used to generate a report without creating a snapshot. Because of the complexity of some reports, not all of them support the Live option.
* **SharePoint Objects** - This is a complex filter that supports the picking of objects from an Office 365 tenant or SharePoint On-Premises on multiple levels. Depending on the report in question it will ask you to choose either a tenant/On-Premise web application or site collections from a tenant. All of the connected site collections will be shown in this filter including Office 365 Groups, Teams and OneDrive site collections. The **Permissions Matrix** and the **Externally Shared Content Matrix** reports use a more advanced configuration of this filter and you can choose a specific securable object in the SharePoint hierarchy. So, to generate the **Permissions Matrix** report for a specific list, you would drag the Filter By slider to _Lists_ and select an object in each of the categories: Tenants, Sites, Subsites, Lists.
* **Content Level** - The Content Level filter lets us choose which types of objects we want to include in the generated report. It is called **Content Level** because the selection of the filter determines the lowest level for which the report will be generated. For example, choosing **Subsites** in the **Permissions Matrix** will result in a report that contains data down to the subsites level. Permission data for lists and list items will not be included.
* **Principals** - The Principals filter is used to filter by principals. Principals include:
  * users
  * security groups, Office 365 Groups
  * SharePoint Groups
  * special groups that represent _Sharing Links_
    * People in the organization with a view sharing link
    * People in the organization with an edit sharing link
    * Anyone with an anonymous view sharing link
    * Anyone with an anonymous edit sharing link
    * Specific people with a sharing link
* **Securable Objects** - By default, reports that show permissions are generated only for objects that have unique permissions or the directly selected objects in the SharePoint Objects filter. Any child objects will have their permissions shown only if they are uniquely secured. This is so as to avoid an explosion of report data because each and every object above or equal to the _Content Level_ filter would be shown along with the associated permissions. If you do wish to see each and every child object along with their permissions \(which would be the same as the parent object by definition\) you can use this filter to modify the report behavior.

## Drill Functionality

Most of the reports are interconnected between each other and with the rest of the application. You can drill from one to the other by using the drill functionality.  
The drill functionality is available when you hover or select a row in a snapshot report and is denoted with a recognizable drill icon. Depending on the report different options to drill will be available. Different rows may also have different drill options and lead to different parts of the application.

For example the **Permissions Matrix** report allows the following:

* if a SharePoint object is selected - switching to live permissions on the **SharePoint Explorer** screen to allow permission management on the object in question
* if a user is selected
  * switching to the **User Permissions Details** Report
  * switching to live permissions on the **SharePoint Explorer** screen to allow permission management on the object where the user has permissions

## Column Chooser

When you select a Security Report that consisits of more columns, you have an option to group them the way you want. You will have the option **Drag columns to group** available on certain reports. After you pick the report you want and generate the data, you can drag the column up to the gray space. When you do this, that column will appear above the rest of the columns, and also if you drag more columns up, data will be shown in a hierarchy, to make reading of the report easier.

