---
UID: NF:winddi.EngUnlockDirectDrawSurface
title: EngUnlockDirectDrawSurface function (winddi.h)
author: windows-sdk-content
description: The EngUnlockDirectDrawSurface function releases the lock on the specified surface.
old-location: display\engunlockdirectdrawsurface.htm
tech.root: display
ms.assetid: 61d1ff1a-d5e3-4542-953c-8b1771622a63
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EngUnlockDirectDrawSurface, EngUnlockDirectDrawSurface function [Display Devices], display.engunlockdirectdrawsurface, gdifncs_6582e033-3e56-4a8d-904d-2978c63ddd4b.xml, winddi/EngUnlockDirectDrawSurface
ms.topic: function
req.header: winddi.h
req.include-header: Winddi.h
req.target-type: Universal
req.target-min-winverclnt: Available in Windows 2000 and later versions of the Windows operating systems.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Win32k.lib
req.dll: Win32k.sys
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Win32k.sys
api_name:
 - EngUnlockDirectDrawSurface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# EngUnlockDirectDrawSurface function


## -description


The <b>EngUnlockDirectDrawSurface</b> function releases the lock on the specified surface.


## -parameters




### -param pSurface [in]

Pointer to a <a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a> structure that describes the surface to be unlocked.


## -returns



<b>EngUnlockDirectDrawSurface</b> returns <b>TRUE</b> when it successfully unlocks the specified surface. Otherwise, it returns <b>FALSE</b>.




## -remarks



The surface must previously have been locked by <a href="https://msdn.microsoft.com/be43afe9-97c9-4ae4-b18c-3312ae757798">EngLockDirectDrawSurface</a>.




## -see-also




<a href="https://msdn.microsoft.com/be43afe9-97c9-4ae4-b18c-3312ae757798">EngLockDirectDrawSurface</a>
 

 

