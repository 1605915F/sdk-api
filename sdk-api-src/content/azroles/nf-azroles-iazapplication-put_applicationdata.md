---
UID: NF:azroles.IAzApplication.put_ApplicationData
title: IAzApplication::put_ApplicationData (azroles.h)
author: windows-sdk-content
description: Sets or retrieves an opaque field that can be used by the application to store information.
old-location: security\iazapplication_applicationdata.htm
tech.root: SecAuthZ
ms.assetid: 7d7ec5c8-8032-437a-92b5-5c578deda6f9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ApplicationData property [Security], ApplicationData property [Security],AzApplication object, ApplicationData property [Security],IAzApplication interface, AzApplication object [Security],ApplicationData property, IAzApplication interface [Security],ApplicationData property, IAzApplication.ApplicationData, IAzApplication.put_ApplicationData, IAzApplication::ApplicationData, IAzApplication::get_ApplicationData, IAzApplication::put_ApplicationData, azroles/IAzApplication::ApplicationData, azroles/IAzApplication::get_ApplicationData, azroles/IAzApplication::put_ApplicationData, put_ApplicationData, security.iazapplication_applicationdata
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
 - IAzApplication.ApplicationData
 - IAzApplication.get_ApplicationData
 - IAzApplication.put_ApplicationData
 - AzApplication.ApplicationData
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzApplication::put_ApplicationData


## -description


The <b>ApplicationData</b> property sets or retrieves an opaque field that can be used by the application to store information.

This property is read/write.


## -parameters


## -remarks



<div class="alert"><b>Important</b>  Policy administrators can read from and write to this property. Applications should not store data in the <b>ApplicationData</b> property that should not be available to the policy administrator.</div>
<div> </div>


