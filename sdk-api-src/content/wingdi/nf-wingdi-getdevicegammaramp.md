---
UID: NF:wingdi.GetDeviceGammaRamp
title: GetDeviceGammaRamp function (wingdi.h)
author: windows-sdk-content
description: The GetDeviceGammaRamp function gets the gamma ramp on direct color display boards having drivers that support downloadable gamma ramps in hardware.
old-location: wcs\getdevicegammaramp.htm
tech.root: WCS
ms.assetid: c32600a9-545e-4bbf-a3c1-21878f5106b0
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetDeviceGammaRamp, GetDeviceGammaRamp function [Windows Color System], _color_GetDeviceGammaRamp, wcs.getdevicegammaramp, wingdi/GetDeviceGammaRamp
ms.topic: function
req.header: wingdi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Gdi32.lib
req.dll: Gdi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - gdi32.dll
 - Ext-MS-Win-GDI-Internal-Desktop-L1-1-0.dll
 - GDI32Full.dll
api_name:
 - GetDeviceGammaRamp
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetDeviceGammaRamp function


## -description


The <b>GetDeviceGammaRamp</b> function gets the <a href="https://msdn.microsoft.com/en-us/library/Dd316909(v=VS.85).aspx">gamma ramp</a> on direct color display boards having drivers that support downloadable gamma ramps in hardware.


## -parameters




### -param hdc

Specifies the device context of the direct color display board in question.


### -param lpRamp

Points to a buffer where the function can place the current gamma ramp of the color display board. The gamma ramp is specified in three arrays of 256 <b>WORD</b> elements each, which contain the mapping between RGB values in the frame buffer and digital-analog-converter (DAC) values. The sequence of the arrays is red, green, blue.


## -returns



If this function succeeds, the return value is <b>TRUE</b>.

If this function fails, the return value is <b>FALSE</b>.




## -remarks



Direct color display modes do not use color lookup tables and are usually 16, 24, or 32 bit. Not all direct color video boards support loadable gamma ramps. <b>GetDeviceGammaRamp</b> succeeds only for devices with drivers that support downloadable gamma ramps in hardware.




## -see-also




<a href="https://msdn.microsoft.com/a0623917-0b63-4546-a71a-1e9efa9fe8e5">Basic Color Management Concepts</a>



<a href="https://msdn.microsoft.com/ee9e9502-5514-4070-95fa-265674a1dde7">Functions</a>
 

 

