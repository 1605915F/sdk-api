---
UID: NF:azroles.IAzApplication.get_DelegatedPolicyUsersName
title: IAzApplication::get_DelegatedPolicyUsersName
author: windows-sdk-content
description: The DelegatedPolicyUsersName property of IAzApplication retrieves the account names of principals that act as delegated policy users.
old-location: security\iazapplication_delegatedpolicyusersname.htm
tech.root: SecAuthZ
ms.assetid: ee18b86f-7ae2-4984-ac7a-3909eda647e3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzApplication object [Security],DelegatedPolicyUsersName property, DelegatedPolicyUsersName property [Security], DelegatedPolicyUsersName property [Security],AzApplication object, DelegatedPolicyUsersName property [Security],IAzApplication interface, IAzApplication interface [Security],DelegatedPolicyUsersName property, IAzApplication.DelegatedPolicyUsersName, IAzApplication.get_DelegatedPolicyUsersName, IAzApplication::DelegatedPolicyUsersName, IAzApplication::get_DelegatedPolicyUsersName, azroles/IAzApplication::DelegatedPolicyUsersName, azroles/IAzApplication::get_DelegatedPolicyUsersName, get_DelegatedPolicyUsersName, security.iazapplication_delegatedpolicyusersname
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
 - IAzApplication.DelegatedPolicyUsersName
 - IAzApplication.get_DelegatedPolicyUsersName
 - AzApplication.DelegatedPolicyUsersName
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzApplication::get_DelegatedPolicyUsersName


## -description


The <b>DelegatedPolicyUsersName</b> property retrieves the account names of principals that act as delegated policy users.

This property is read-only.


## -parameters


## -remarks



Delegated policy users are principals that are allowed to read the subset of the policy data that the policy administrator of an <a href="https://msdn.microsoft.com/ea4a8a84-5003-44da-b75e-34da6bd898dd">IAzApplication</a> object uses to administer the delegated object.

<div class="alert"><b>Note</b>  Delegated policy users are not supported for XML stores.</div>
<div> </div>
In JScript, the returned <a href="https://msdn.microsoft.com/en-us/library/ms221482(v=VS.85).aspx">SAFEARRAY</a> must be converted to the JScript <a href="https://msdn.microsoft.com/library/k4h76zbx(v=VS.85).aspx">Array</a> object. 



