---
UID: NF:wscapi.WscUnRegisterChanges
title: WscUnRegisterChanges function (wscapi.h)
author: windows-sdk-content
description: Cancels a callback registration that was made by a call to the WscRegisterForChanges function.
old-location: winprog\wscunregisterchanges.htm
tech.root: DevNotes
ms.assetid: cfb0d076-bd8b-4483-a036-51c77b8181c9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WscUnRegisterChanges, WscUnRegisterChanges function [Windows API], winprog.wscunregisterchanges, wscapi/WscUnRegisterChanges
ms.topic: function
req.header: wscapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wscapi.lib
req.dll: Wscapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Wscapi.dll
api_name:
 - WscUnRegisterChanges
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WscUnRegisterChanges function


## -description


Cancels a callback registration that was made by a call to the <a href="https://msdn.microsoft.com/55f2d281-6308-4344-98dc-3b1c7cbee9df">WscRegisterForChanges</a> function.


## -parameters




### -param hRegistrationHandle [in]

The handle to the registration context returned as the <i>phCallbackRegistration</i> of the <a href="https://msdn.microsoft.com/55f2d281-6308-4344-98dc-3b1c7cbee9df">WscRegisterForChanges</a> function.


## -returns



Returns <b>S_OK</b> if the function succeeds, otherwise returns an error code.




## -see-also




<a href="https://msdn.microsoft.com/55f2d281-6308-4344-98dc-3b1c7cbee9df">WscRegisterForChanges</a>
 

 

