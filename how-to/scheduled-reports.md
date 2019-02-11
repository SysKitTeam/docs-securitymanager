---
title: Schedule Reports 

description: This article describes what are and how to use Schedule Reports.  

author: Tea Bašić 

date: 11/02/2019 

--- 
# Send Scheduled Reports

This article explains how to use __Scheduled Reports__ to schedule sending SysKit Security Manager reports to the desired email addresses or for upload to a SharePoint document library. In order to use this feature, you have to turn it on in the Settings menu. There you can also change prefered time of day to send reports and email settings.  


 If you installed the application [default way](#internal/installation/installation-guide), then the Report Sets will be sent if the application is turned on or minimized in the tray. If you turn on the application within 24 hours what the reports should have been sent, the scheduled reports will be sent then.  

 

On __Scheduled Reports Screen__ you can see all created report sets, their destination, when was the last run time, frequency and scheduling date. Also you can create new Report Sets and access schedule options. If you hoover over one of the Report Sets on the right corner you get 3 additional buttons – Edit button, Delete button and Send now. 

  

## Create new Report Set 

This section describes how to create scheduled __Report Sets__  in SysKit Security Manager. Data you receive from these reports is gathered from the __latest loaded snapshot__ information. 

  

If you wish to use __Scheduled reports__ feature, please make sure you configured the [Scheduled Settings](#internal/get-to-know-security-manager/settings-screen) properly. 

   

1.  Set name and schedule on which reports will be sent. Available delivery periods are __daily, weekly__ , __monthly__ and __after scheduled snapshot is finished__ . Exact time can be changed in scheduled settings.  

  

1. Choose delivery options: 

    * __Email__ –   Required fields are __Send To and Body__. Provide the email address to which you wish to send the subscription. You can enter more recipients – just separate the email addresses with semicolons. Type in the subject and body text. 

 

On default is set on Exchange Online which means that Report Set will be sent via Exchange Online on behalf of current user.  In scheduled settings you can set up __Outgoing Email server__. That way email will be sent through existing email server using the supplied information.   

__Please note!__ – If you don't set up outgoing email server, reports for the on premise SharePoint can't be sent via e-mail.  

 

    * __SharePoint Library__ 

   

You can select both delivery methods. Report Sets will be sent to the email addresses you provided and uploaded to the SharePoint document library. 

  

1. Choose Report from available __Security Reports__. 

  

For certain reports, you will have to adjust filters to complete the report configuration. The filters will define the data displayed in the report. Click __Add__ to add the selected report to the subscription. 

  

1. You can add more reports by repeating previous steps or delete added reports. 

  

1. Click __Finish__ to create Report Set and exit.  

  

There are two ways to create new Report Set: 

* On the Scheduled reports Screen 

  

* On the Security Reports Screen, or more precisely on each individual report screen there is a button to schedule report of that specific report and you can choose to create new report or to add to existing one. This way step 4. and 5. are skipped because report is already selected. 

