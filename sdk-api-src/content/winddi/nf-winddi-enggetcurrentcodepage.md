---
UID: NF:winddi.EngGetCurrentCodePage
title: EngGetCurrentCodePage function (winddi.h)
author: windows-sdk-content
description: The EngGetCurrentCodePage function returns the system's default OEM and ANSI code pages.
old-location: display\enggetcurrentcodepage.htm
tech.root: display
ms.assetid: d53a1b6b-40b1-42a5-acfe-4b17f24d00c1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EngGetCurrentCodePage, EngGetCurrentCodePage function [Display Devices], display.enggetcurrentcodepage, gdifncs_39440cc8-e1f5-4f88-b92a-d8a7eb3d1d39.xml, winddi/EngGetCurrentCodePage
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
 - Ext-MS-Win-GDI-Internal-Desktop-L1-1-0.dll
 - GDI32.dll
 - GDI32Full.dll
api_name:
 - EngGetCurrentCodePage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# EngGetCurrentCodePage function


## -description


The <b>EngGetCurrentCodePage</b> function returns the system's default OEM and ANSI code pages.


## -parameters




### -param OemCodePage [out]

Pointer to a USHORT that receives the system's default OEM code page.


### -param AnsiCodePage [out]

Pointer to a USHORT that receives the system's default ANSI code page.


## -returns



None




## -remarks



<b>EngGetCurrentCodePage</b> returns the default code pages that are used by the system to translate from ANSI to Unicode. These values are set at boot time according to locale settings.




## -see-also




<a href="https://msdn.microsoft.com/b28e5854-1ac0-4b76-87a9-ec943228e2ed">STROBJ_dwGetCodePage</a>
 

 

