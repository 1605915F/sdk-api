---
UID: NF:azroles.IAzAuthorizationStore.get_DelegatedPolicyUsersName
title: IAzAuthorizationStore::get_DelegatedPolicyUsersName
author: windows-sdk-content
description: Retrieves the account names of principals that act as delegated policy users.
old-location: security\azauthorizationstore_delegatedpolicyusersname.htm
tech.root: SecAuthZ
ms.assetid: 495cdba4-7127-48aa-9542-7ccbedbad589
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzAuthorizationStore object [Security],DelegatedPolicyUsersName property, DelegatedPolicyUsersName property [Security], DelegatedPolicyUsersName property [Security],AzAuthorizationStore object, DelegatedPolicyUsersName property [Security],IAzAuthorizationStore interface, IAzAuthorizationStore interface [Security],DelegatedPolicyUsersName property, IAzAuthorizationStore.DelegatedPolicyUsersName, IAzAuthorizationStore.get_DelegatedPolicyUsersName, IAzAuthorizationStore::DelegatedPolicyUsersName, IAzAuthorizationStore::get_DelegatedPolicyUsersName, azroles/IAzAuthorizationStore::DelegatedPolicyUsersName, azroles/IAzAuthorizationStore::get_DelegatedPolicyUsersName, get_DelegatedPolicyUsersName, security.azauthorizationstore_delegatedpolicyusersname
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
 - IAzAuthorizationStore.DelegatedPolicyUsersName
 - IAzAuthorizationStore.get_DelegatedPolicyUsersName
 - AzAuthorizationStore.DelegatedPolicyUsersName
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzAuthorizationStore::get_DelegatedPolicyUsersName


## -description


The <b>DelegatedPolicyUsersName</b> property retrieves the account names of principals that act as delegated policy users.

This property is read-only.


## -parameters


## -remarks



Delegated policy users are principals that are allowed to read the subset of the policy data that the policy administrator of an <a href="https://msdn.microsoft.com/ea4a8a84-5003-44da-b75e-34da6bd898dd">IAzApplication</a>  or <a href="https://msdn.microsoft.com/f7abe7cb-8827-46f6-85fe-99282582a3d4">IAzScope</a> object uses to administer the delegated object.

<div class="alert"><b>Note</b>  Delegated policy users are not supported for XML stores.</div>
<div> </div>
In  JScript, the returned <a href="https://msdn.microsoft.com/en-us/library/ms221482(v=VS.85).aspx">SAFEARRAY</a> must be converted to the JScript <a href="https://msdn.microsoft.com/library/k4h76zbx(v=VS.85).aspx">Array</a> object. 



