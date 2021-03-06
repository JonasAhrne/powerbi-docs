---
title: How admins can manage the Power BI Desktop sign-in form
description: Learn how you can manage the initial sign-in form when opening Power BI Desktop.
author: davidiseminger
ms.reviewer: ''

ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 04/15/2019
ms.author: davidi

---
# Administrators: Manage the Power BI Desktop sign-in form
The first time Power BI Desktop is launched, a sign-in form is displayed. Information can be filled in, or sign in to Power BI to continue. Administrators manage this form by using a registry key. 

![Initial sign-in form for Power BI Desktop](media/desktop-admin-sign-in-form/sign-in-form.png)

Administrators use the following registry key to disable the sign-in form. This can also be pushed to an entire organization by using global policies.

```
Key: HKEY_CURRENT_USER\SOFTWARE\Policies\Microsoft\Microsoft Power BI Desktop
valueName: ShowLeadGenDialog
```
You can also try the following key, which has been successful for some customers based on their configurations:

```
Key: HKEY_CURRENT_USER\SOFTWARE\Microsoft\Microsoft Power BI Desktop
valueName: ShowLeadGenDialog
```

A value of 0 will disable the dialog.




More questions? [Try asking the Power BI Community](https://community.powerbi.com/)

