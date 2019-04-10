---
UID: NF:wingdi.MoveToEx
title: MoveToEx function (wingdi.h)
author: windows-sdk-content
description: The MoveToEx function updates the current position to the specified point and optionally returns the previous position.
old-location: gdi\movetoex.htm
tech.root: gdi
ms.assetid: af11eeb7-4036-4a90-8685-9b5719f79e01
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: MoveToEx, MoveToEx function [Windows GDI], _win32_MoveToEx, gdi.movetoex, wingdi/MoveToEx
ms.topic: function
req.header: wingdi.h
req.include-header: Windows.h
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
 - Ext-MS-Win-GDI-Draw-l1-1-0.dll
 - Ext-MS-Win-GDI-Draw-l1-1-1.dll
 - ext-ms-win-gdi-draw-l1-1-2.dll
 - Ext-MS-Win-GDI-Draw-L1-1-3.dll
 - GDI32Full.dll
api_name:
 - MoveToEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MoveToEx function


## -description


The <b>MoveToEx</b> function updates the current position to the specified point and optionally returns the previous position.


## -parameters




### -param hdc [in]

Handle to a device context.


### -param x [in]

Specifies the x-coordinate, in logical units, of the new position, in logical units.


### -param y [in]

Specifies the y-coordinate, in logical units, of the new position, in logical units.


### -param lppt [out]

Pointer to a <a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a> structure that receives the previous current position. If this parameter is a <b>NULL</b> pointer, the previous position is not returned.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero.




## -remarks



The <b>MoveToEx</b> function affects all drawing functions.


#### Examples

For an example, see <a href="https://msdn.microsoft.com/69114875-f3e0-45e9-8e87-1f4e9de08db1">Drawing Markers</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/65c38da1-ab7d-4e80-83e3-ba1db66f8fd9">AngleArc</a>



<a href="https://msdn.microsoft.com/90f123e2-c3c7-4ba1-a42b-7d6bc0074d5b">Line and Curve Functions</a>



<a href="https://msdn.microsoft.com/a31b3a9a-110f-4cdf-89d9-19937a2e40b4">LineTo</a>



<a href="https://msdn.microsoft.com/8c65c185-8346-459e-bdf7-1cf3f7419736">Lines and Curves Overview</a>



<a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a>



<a href="https://msdn.microsoft.com/0c8d6d6d-d0a3-4188-91ad-934e6f054862">PolyBezierTo</a>



<a href="https://msdn.microsoft.com/76020742-b651-4244-82c3-13034573c306">PolylineTo</a>
 

 

