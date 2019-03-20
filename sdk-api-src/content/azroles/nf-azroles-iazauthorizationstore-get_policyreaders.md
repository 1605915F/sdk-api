---
UID: NF:azroles.IAzAuthorizationStore.get_PolicyReaders
title: IAzAuthorizationStore::get_PolicyReaders (azroles.h)
author: windows-sdk-content
description: Retrieves the security identifiers (SIDs) of principals that act as policy readers in text form.
old-location: security\azauthorizationstore_policyreaders.htm
tech.root: SecAuthZ
ms.assetid: 22479ced-b393-40d3-bb16-f3c3e595dacf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzAuthorizationStore object [Security],PolicyReaders property, IAzAuthorizationStore interface [Security],PolicyReaders property, IAzAuthorizationStore.PolicyReaders, IAzAuthorizationStore.get_PolicyReaders, IAzAuthorizationStore::PolicyReaders, IAzAuthorizationStore::get_PolicyReaders, PolicyReaders property [Security], PolicyReaders property [Security],AzAuthorizationStore object, PolicyReaders property [Security],IAzAuthorizationStore interface, azroles/IAzAuthorizationStore::PolicyReaders, azroles/IAzAuthorizationStore::get_PolicyReaders, get_PolicyReaders, security.azauthorizationstore_policyreaders
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
 - IAzAuthorizationStore.PolicyReaders
 - IAzAuthorizationStore.get_PolicyReaders
 - AzAuthorizationStore.PolicyReaders
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzAuthorizationStore::get_PolicyReaders


## -description


The <b>PolicyReaders</b> property retrieves the <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifiers</a> (SIDs) of principals that act as policy readers in text form.

This property is read-only.


## -parameters


## -remarks



Policy readers for an object can read attributes for the object and for child objects of the object. Readers can also  use the policy; for example, readers can call the <a href="https://msdn.microsoft.com/0bd16cdb-3dba-4656-b264-32e622732155">AccessCheck</a> method. Readers cannot modify the object or its child objects.

In  JScript, the returned <a href="https://msdn.microsoft.com/en-us/library/ms221482(v=VS.85).aspx">SAFEARRAY</a> must be converted to the JScript <a href="https://msdn.microsoft.com/library/k4h76zbx(v=VS.85).aspx">Array</a> object. 



