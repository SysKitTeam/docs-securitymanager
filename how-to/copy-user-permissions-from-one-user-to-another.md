---
description: >-
  This section describes how to copy user permissions from one user to another
  using SysKit Security Manager.
---

# Copy user permissions from one user to another

Managing user's permissions is very important regarding both Office 365 and SharePoint. When it comes to copying permissions from one user to another, you do not have a simple solution in the **Microsoft 365 admin center**.

A user may be granted permissions on various levels with different access rights. It would become very time-consuming to find and grant the same level of permissions to multiple users.

There are two common strategies to this problem:

* You can create a group and assign certain permissions to it. This way you assure identical permissions for all users by simply adding them to the same group.
* The other way is to use a custom **PowerShell** script.

The best solution for this problem is to use **SysKit Security Manager** and copy permissions in a few mouse clicks. Here are the required steps:

From the **Overview** screen, click on **Users**.

![](../.gitbook/assets/how-to-copy-user-permissions-from-one-user-to-another_ssm_01.png)

Select the **Single User** report from the section **Explore & Manage**. 

1. Make sure to choose the right point in time from which you wish to copy user permissions to other users. If you want the latest permissions copied, choose **the newest snapshot**. 
2. In case you have multiple **tenants**, ****choose the appropriate one from the drop down menu.
3. Select **the user** which you want to use as a source for copying the permissions.

![](../.gitbook/assets/how-to-copy-user-permissions-from-one-user-to-another_ssm_02.png)

On the **Sites** tab of the **Single User** report, you will find a list of all the places where the selected user has any kind of access or granted permissions. This includes:

* Classic site collections
* Office 365 Groups&Teams
* OneDrive sites

Once you choose, for example the **/sites/cw,** site collection, two available actions that are related to the selected user will appear on the top of the grid. Available actions are:

* **Remove User** - Remove the selected user from all of the selected site collection\(s\).
* **Copy Permissions** - Copy permissions and group memberships of the currently selected user to a different one on the selected site\(s\). Before performing an action, a user has two additional options available:
  * **Copy Site Administrator role** - if the source principal is the site collection administrator of the selected site\(s\), the target user will be added as the site administrator as well. 
  * **Keep existing destination principal\(s\) permissions and group membership** - the destination principals\(s\) will acquire all permissions and group membership\(s\) from the source principal without loosing the ones he had before this action.

{% hint style="warning" %}
**Please note!** The following limitations may apply: sharing links, OneDrive access, and Security Groups membership will not be copied.
{% endhint %}

![](../.gitbook/assets/how-to-copy-user-permissions-from-one-user-to-another_ssm_03.png)

Once you click on the **Copy Permissions,** you will be asked to select **Destination Principal\(s\)** and mark the checkboxes if they are applicable for your action.

![](../.gitbook/assets/how-to-copy-user-permissions-from-one-user-to-another_ssm_04.png)

You can choose one or multiple destination principals. Click on the **Copy** button to start with this action.

![](../.gitbook/assets/how-to-copy-user-permissions-from-one-user-to-another_ssm_05.png)

Once that the action starts, you can track the information about copying of the permission progress in the lower right corner.

![](../.gitbook/assets/how-to-copy-user-permissions-from-one-user-to-another_ssm_06.png)

**Tips and tricks**: If you wish to copy all the permissions of one user, mark a checkbox next to the **Name** column and select the **Copy Permissions** action.

![](../.gitbook/assets/how-to-copy-user-permissions-from-one-user-to-another_ssm_07.png)

