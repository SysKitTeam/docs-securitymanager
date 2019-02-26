---
description: >-
  This section describes how to connect to a single or multiple SharePoint
  On-Premise site collections from SysKit Security Manager.
---

# Connect to SharePoint On-Premise Site Collections

Choose SharePoint **On-Premise** to start the connection wizard.

## Credentials

You can choose to login using either the **Integrated Security** or enter the credentials in a format: "Domain\Username". Then click the **Test Credentials** button and **Next** to proceed.

## Flow Selection

If you are a **Farm Administrator**, you’ll be able to automatically discover all site collections in a selected farm.  
Enter **SharePoint Configuration Database** details. Click **Test Connection** button and then **Discover**.

If you are a **Site Collection Administrator**, you can connect to site collections manually.

## Site Collections

If you are a **Farm Administrator**, all site collections from your farm will be auto-discovered and you’ll be able to select site collections you want to manage.

If you are a **Site Collection Administrator** you can:

1. Connect to on-premises site collection by **entering its URL** or
2. **import a text file with site collection URLs**, newline separated.
3. Click the **Test Connection** button and **Next** to proceed.

{% hint style="warning" %}
If you choose the **Import from file** option, you’ll be able to download the PowerShell script, which will generate a .txt file that you can import. Copy the downloaded script on the SharePoint server, execute it and then import the file in the SysKit Security Manager.
{% endhint %}

## Summary

Here is an overview of all the site collections that will be added. You can always edit these from the main navigation.

