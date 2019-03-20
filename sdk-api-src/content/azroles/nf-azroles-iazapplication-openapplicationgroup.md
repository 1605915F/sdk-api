---
UID: NF:azroles.IAzApplication.OpenApplicationGroup
title: IAzApplication::OpenApplicationGroup (azroles.h)
author: windows-sdk-content
description: Opens an IAzApplicationGroup object by specifying its name.
old-location: security\iazapplication_openapplicationgroup.htm
tech.root: SecAuthZ
ms.assetid: 6f9c9d65-73aa-40e9-bd04-d4d5d4370201
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AzApplication object [Security],OpenApplicationGroup method, IAzApplication interface [Security],OpenApplicationGroup method, IAzApplication.OpenApplicationGroup, IAzApplication::OpenApplicationGroup, OpenApplicationGroup, OpenApplicationGroup method [Security], OpenApplicationGroup method [Security],AzApplication object, OpenApplicationGroup method [Security],IAzApplication interface, azroles/IAzApplication::OpenApplicationGroup, security.iazapplication_openapplicationgroup
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
 - IAzApplication.OpenApplicationGroup
 - AzApplication.OpenApplicationGroup
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# IAzApplication::OpenApplicationGroup


## -description


The <b>OpenApplicationGroup</b> method opens an <a href="https://msdn.microsoft.com/6a15acde-e582-4c49-b7e4-82d4e54012b1">IAzApplicationGroup</a> object with the specified name.


## -parameters




### -param bstrGroupName [in]

Name of the <a href="https://msdn.microsoft.com/6a15acde-e582-4c49-b7e4-82d4e54012b1">IAzApplicationGroup</a> object to open.


### -param varReserved [in, optional]

Reserved for future use.


### -param ppGroup [out]

A pointer to a pointer to the opened <a href="https://msdn.microsoft.com/6a15acde-e582-4c49-b7e4-82d4e54012b1">IAzApplicationGroup</a> object.


## -returns



 If the method succeeds, the method returns S_OK.

Any other <b>HRESULT</b> value indicates that the operation failed.



