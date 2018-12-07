---
UID: NF:azroles.IAzAuthorizationStore.Submit
title: IAzAuthorizationStore::Submit
author: windows-sdk-content
description: Persists changes made to the AzAuthorizationStore object.
old-location: security\azauthorizationstore_submit.htm
tech.root: secauthz
ms.assetid: bf2962af-0e8f-4c4c-a63a-dfd623308e4d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzAuthorizationStore object [Security],Submit method, IAzAuthorizationStore interface [Security],Submit method, IAzAuthorizationStore.Submit, IAzAuthorizationStore::Submit, Submit, Submit method [Security], Submit method [Security],AzAuthorizationStore object, Submit method [Security],IAzAuthorizationStore interface, azroles/IAzAuthorizationStore::Submit, security.azauthorizationstore_submit
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - AzAuthorizationStore.Submit
 - IAzAuthorizationStore.Submit
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzAuthorizationStore::Submit


## -description


The <b>Submit</b> method persists changes made to the <a href="https://msdn.microsoft.com/en-us/library/Aa376327(v=VS.85).aspx">AzAuthorizationStore</a> object.


## -parameters




### -param lFlags [in]

Flags that modify the behavior of the <b>Submit</b> method. The default value is zero. If the AZ_SUBMIT_FLAG_ABORT flag is specified, the changes to the object are discarded and the object is updated to match the underlying policy store.


### -param varReserved [in, optional]

Reserved for future use.


## -remarks



Any additions or modifications to an <a href="https://msdn.microsoft.com/en-us/library/Aa376327(v=VS.85).aspx">AzAuthorizationStore</a> object are not persisted until the <b>Submit</b> method is called. The <a href="https://msdn.microsoft.com/en-us/library/Aa376345(v=VS.85).aspx">Delete</a>  method automatically submits changes.

The <b>Submit</b> method does not extend to child objects; child objects  must be individually persisted to the policy store. A created <a href="https://msdn.microsoft.com/en-us/library/Aa376327(v=VS.85).aspx">AzAuthorizationStore</a> object must be submitted before it can be referenced or become a parent object. The destructor for an object silently discards unsubmitted changes.



