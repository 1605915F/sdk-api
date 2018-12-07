---
UID: NF:gdiplusgraphics.Graphics.IsVisible(IN REAL,IN REAL)
title: Graphics::IsVisible(IN REAL,IN REAL)
author: windows-sdk-content
description: The Graphics::IsVisible method determines whether the specified point is inside the visible clipping region of this Graphics object.
old-location: gdiplus\_gdiplus_CLASS_Graphics_IsVisible_REAL_x_REAL_y_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\graphicsisvisiblemethods\isvisible_14realx_realy.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Graphics class [GDI+],IsVisible method, Graphics.IsVisible, Graphics.IsVisible(IN REAL,IN REAL), Graphics.IsVisible(REAL,REAL), Graphics::IsVisible, Graphics::IsVisible(IN REAL,IN REAL), IsVisible, IsVisible method [GDI+], IsVisible method [GDI+],Graphics class, _gdiplus_CLASS_Graphics_IsVisible_REAL_x_REAL_y_, gdiplus._gdiplus_CLASS_Graphics_IsVisible_REAL_x_REAL_y_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusgraphics.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
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
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gdiplus.dll
api_name:
 - Graphics.IsVisible
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Graphics::IsVisible(IN REAL,IN REAL)


## -description


The <b>Graphics::IsVisible</b> method determines whether the specified point is inside the visible clipping region of this <a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a> object. The visible clipping region is the intersection of the clipping region of this <b>Graphics</b> object and the clipping region of the window.


## -parameters




### -param x [in]

Type: <b>REAL</b>

Real number that specifies the x-coordinate of the point to test. 


### -param y [in]

Type: <b>REAL</b>

Real number that specifies the y-coordinate of the point to test. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the specified coordinates are inside the visible clipping region, this method returns <b>TRUE</b>; otherwise, it returns <b>FALSE</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>



<a href="https://msdn.microsoft.com/73733baf-6cbf-4220-b89d-0cd6856acc46">Graphics::IsVisibleClipEmpty</a>
 

 

