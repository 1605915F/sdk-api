---
UID: NF:winuser.SetRect
title: SetRect function (winuser.h)
author: windows-sdk-content
description: The SetRect function sets the coordinates of the specified rectangle. This is equivalent to assigning the left, top, right, and bottom arguments to the appropriate members of the RECT structure.
old-location: gdi\setrect.htm
tech.root: gdi
ms.assetid: 346c573b-eaf7-4ca6-bd36-18074f7eccf5
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SetRect, SetRect function [Windows GDI], _win32_SetRect, gdi.setrect, winuser/SetRect
ms.topic: function
req.header: winuser.h
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
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - user32.dll
 - API-MS-Win-NTUser-Rectangle-l1-1-0.dll
 - minuser.dll
 - Ext-MS-Win-NTUser-Rectangle-Ext-l1-1-0.dll
api_name:
 - SetRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetRect function


## -description


The <b>SetRect</b> function sets the coordinates of the specified rectangle. This is equivalent to assigning the left, top, right, and bottom arguments to the appropriate members of the <b>RECT</b> structure.


## -parameters




### -param lprc [out]

Pointer to the <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that contains the rectangle to be set.


### -param xLeft [in]

Specifies the x-coordinate of the rectangle's upper-left corner.


### -param yTop [in]

Specifies the y-coordinate of the rectangle's upper-left corner.


### -param xRight [in]

Specifies the x-coordinate of the rectangle's lower-right corner.


### -param yBottom [in]

Specifies the y-coordinate of the rectangle's lower-right corner.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero.




## -remarks



Because applications can use rectangles for different purposes, the rectangle functions do not use an explicit unit of measure. Instead, all rectangle coordinates and dimensions are given in signed, logical values. The mapping mode and the function in which the rectangle is used determine the units of measure.


#### Examples

For an example, see <a href="https://msdn.microsoft.com/e8861240-9345-43e6-820d-d237247d1bd7">Using Rectangles</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/9349ba83-59d6-49d0-ac9d-a4d9589748dd">CopyRect</a>



<a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a>



<a href="https://msdn.microsoft.com/b03da8c9-ee6d-4045-8d90-8beceb09ead5">Rectangle Functions</a>



<a href="https://msdn.microsoft.com/23c251d1-b8c5-425f-b2b3-44954cf653e9">Rectangles Overview</a>



<a href="https://msdn.microsoft.com/d3c677ae-e45c-4d54-8521-75954a466a68">SetRectEmpty</a>
 

 

