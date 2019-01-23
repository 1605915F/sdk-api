---
UID: NF:azroles.IAzScope.get_PolicyAdministratorsName
title: IAzScope::get_PolicyAdministratorsName
author: windows-sdk-content
description: Retrieves the account names of principals that act as policy administrators.
old-location: security\iazscope_policyadministratorsname.htm
tech.root: SecAuthZ
ms.assetid: 291aa2f8-f08e-45f5-ade7-b456c962dd3f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzScope object [Security],PolicyAdministratorsName property, IAzScope interface [Security],PolicyAdministratorsName property, IAzScope.PolicyAdministratorsName, IAzScope.get_PolicyAdministratorsName, IAzScope::PolicyAdministratorsName, IAzScope::get_PolicyAdministratorsName, PolicyAdministratorsName property [Security], PolicyAdministratorsName property [Security],AzScope object, PolicyAdministratorsName property [Security],IAzScope interface, azroles/IAzScope::PolicyAdministratorsName, azroles/IAzScope::get_PolicyAdministratorsName, get_PolicyAdministratorsName, security.iazscope_policyadministratorsname
ms.topic: method
req.header: azroles.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Azroles.lib
req.dll: Azroles.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Azroles.dll
api_name:
 - IAzScope.PolicyAdministratorsName
 - IAzScope.get_PolicyAdministratorsName
 - AzScope.PolicyAdministratorsName
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzScope::get_PolicyAdministratorsName


## -description


The <b>PolicyAdministratorsName</b> property retrieves the account names of principals that act as policy administrators.

This property is read-only.


## -parameters


## -remarks



Policy administrators for an object can perform the following tasks:

<ul>
<li>Read the object</li>
<li>Write attributes to the object</li>
<li>Read attributes of child objects of the object</li>
<li>Write attributes to child objects of the object</li>
<li>Delete the object</li>
<li>Delete child objects of the object</li>
<li>Create child objects of the object</li>
</ul>
In JScript, the returned <a href="https://msdn.microsoft.com/en-us/library/ms221482(v=VS.85).aspx">SAFEARRAY</a> must be converted to the JScript <a href="https://msdn.microsoft.com/library/k4h76zbx(v=VS.85).aspx">Array</a> object. 



