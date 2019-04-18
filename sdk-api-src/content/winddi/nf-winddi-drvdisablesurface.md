---
UID: NF:winddi.DrvDisableSurface
title: DrvDisableSurface function (winddi.h)
author: windows-sdk-content
description: The DrvDisableSurface function is used by GDI to notify a driver that the surface created by DrvEnableSurface for the current device is no longer needed.
old-location: display\drvdisablesurface.htm
tech.root: display
ms.assetid: 18714107-7287-4d50-a2f9-b5d72f111f8b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DrvDisableSurface, DrvDisableSurface function [Display Devices], ddifncs_1b5543ca-2860-4383-a2a7-a73adc5cf2a4.xml, display.drvdisablesurface, winddi/DrvDisableSurface
ms.topic: function
req.header: winddi.h
req.include-header: Winddi.h
req.target-type: Desktop
req.target-min-winverclnt: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - winddi.h
api_name:
 - DrvDisableSurface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# DrvDisableSurface function


## -description


The <b>DrvDisableSurface</b> function is used by GDI to notify a driver that the surface created by <a href="https://msdn.microsoft.com/a838a44a-243c-4d0d-bda3-eec9a626cb53">DrvEnableSurface</a> for the current device is no longer needed.


## -parameters




### -param dhpdev

Handle to the physical device's <a href="https://msdn.microsoft.com/139a10e9-203b-499b-9291-8537eae9189c">PDEV</a>. This is the handle to the device whose surface is to be released.


## -returns



None




## -remarks



The driver should free any memory and resources used by the surface associated with the PDEV as soon as the physical device is disabled.

If the driver has been disabled by a call to <a href="https://msdn.microsoft.com/29846ffd-b721-4d61-9983-07a2575f9fe8">DrvAssertMode</a>, the driver must not access the hardware during <b>DrvDisableSurface</b> because another active PDEV might be in use. Any necessary hardware changes should have been performed during the call to <b>DrvAssertMode</b>. A driver should keep track of whether it has been disabled by <b>DrvAssertMode</b> so that it can perform proper cleanup operations in <b>DrvDisableSurface</b>.

If the physical device has an enabled surface, GDI calls <b>DrvDisableSurface</b> before calling <a href="https://msdn.microsoft.com/dff04000-e307-4a1c-80fe-d6666929df76">DrvDisablePDEV</a>.

<b>DrvDisableSurface</b> is required for graphics drivers.




## -see-also




<a href="https://msdn.microsoft.com/29846ffd-b721-4d61-9983-07a2575f9fe8">DrvAssertMode</a>



<a href="https://msdn.microsoft.com/8f12cc40-6cff-4e40-a264-58d16d3e55bd">DrvDisableDriver</a>



<a href="https://msdn.microsoft.com/dff04000-e307-4a1c-80fe-d6666929df76">DrvDisablePDEV</a>



<a href="https://msdn.microsoft.com/a838a44a-243c-4d0d-bda3-eec9a626cb53">DrvEnableSurface</a>
 

 

