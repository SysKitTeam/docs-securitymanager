# Send Scheduled Reports

## Scheduled Reports

In order to use this feature, you have to turn it on in the[ Settings](../get-to-know-security-manager/settings-screen.md#schedule-options) menu. There you can also change preferred time of day to send reports and email settings.

On the [Scheduled Reports Screen](../get-to-know-security-manager/scheduled-reports-screen.md) you can see all created report sets, their destination, when was the last run time, frequency and scheduling date. Also you can create new report sets and access [schedule options](../get-to-know-security-manager/settings-screen.md#schedule-options). If you hover over one of the report sets, on the right corner you will get additional options – Edit, Delete and Send now.

{% hint style="info" %}
If you installed the application using the [default](../installation/installation-guide.md#installation-steps) way, Report Sets will be sent while the application is turned on or [minimized in the tray](../get-to-know-security-manager/settings-screen.md#general-settings). If the application was not running at the scheduled time, Report Sets will still be sent upon turning on the application within 24 hours.
{% endhint %}

### Create a new Report Set

This section describes how to create scheduled **Report Sets** in SysKit Security Manager. Data you receive from these reports is gathered from the **latest loaded snapshot** information.

There are two ways to create new Report Set:

* On the [Scheduled Reports](../get-to-know-security-manager/scheduled-reports-screen.md) screen 
* On the [Security Reports](../get-to-know-security-manager/permissions-reports-screen.md) screen: more precisely on each individual report screen there is a button to schedule report of that specific report and you can choose to **create a new report set** or to **add to existing** one.

If you wish to use **Scheduled reports** feature, make sure you configured the [Scheduled Settings](send-scheduled-reports.md#internal/get-to-know-security-manager/settings-screen/#scheduled) properly.

1. Set name and schedule on which reports will be sent. Available delivery periods are **daily, weekly** and **monthly**. Exact time can be changed in[ scheduled settings](../get-to-know-security-manager/settings-screen.md#schedule-options).  
2. Choose delivery options:

* **Email**
  * Required fields are **Send To** and **Body**. Provide the **Email Address** to which you wish to send the subscription. You can enter more recipients – just separate the email addresses with semicolons. Type in the **Subject** and **Body** text. 
  * On default is set on **Exchange Online** which means that Report Set will be sent via Exchange Online on behalf of current user. In [scheduled settings](../get-to-know-security-manager/settings-screen.md#schedule-options) you can set up **Outgoing Email server**. That way email will be sent through existing email server using the supplied information.

{% hint style="warning" %}
**Please note!** If you don't set up outgoing email server, reports for the On-Prem SharePoint can't be sent via e-mail.
{% endhint %}

* **SharePoint Library** 
  * Report Sets will be uploaded to the SharePoint document library.

You can select both delivery methods. Report Sets will be sent to the email addresses you provided and uploaded to the SharePoint document library.

4. Choose wanted Report from available **Security Reports**. 

For certain reports, you will have to adjust [filters](use-filters-drill-and-column-chooser.md#filters) to complete the report configuration. The filters will define the data displayed in the report. Click **Add** to add the selected report to the subscription.

5. You can add more reports by repeating previous steps or delete added reports. 

6. Click **Finish** to create Report Set and exit.  



