---
UID: NF:gdiplusgraphics.Graphics.FillEllipse(IN const Brush,IN REAL,IN REAL,IN REAL,IN REAL)
title: Graphics::FillEllipse(IN const Brush,IN REAL,IN REAL,IN REAL,IN REAL)
author: windows-sdk-content
description: The Graphics::FillEllipse method uses a brush to fill the interior of an ellipse that is specified by coordinates and dimensions.
old-location: gdiplus\_gdiplus_CLASS_Graphics_FillEllipse_Brush_brush_REAL_x_REAL_y_REAL_width_REAL_height_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\graphicsfillellipsemethods\fillellipse_53brushbrush_realx_realy_realwidth_realh.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FillEllipse, FillEllipse method [GDI+], FillEllipse method [GDI+],Graphics class, Graphics class [GDI+],FillEllipse method, Graphics.FillEllipse, Graphics.FillEllipse(IN const Brush,IN REAL,IN REAL,IN REAL,IN REAL), Graphics.FillEllipse(const Brush*,REAL,REAL,REAL,REAL), Graphics::FillEllipse, Graphics::FillEllipse(IN const Brush,IN REAL,IN REAL,IN REAL,IN REAL), _gdiplus_CLASS_Graphics_FillEllipse_Brush_brush_REAL_x_REAL_y_REAL_width_REAL_height_, gdiplus._gdiplus_CLASS_Graphics_FillEllipse_Brush_brush_REAL_x_REAL_y_REAL_width_REAL_height_
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
 - Graphics.FillEllipse
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Graphics::FillEllipse(IN const Brush,IN REAL,IN REAL,IN REAL,IN REAL)


## -description


The <b>Graphics::FillEllipse</b> method uses a brush to fill the interior of an ellipse that is specified by coordinates and dimensions.


## -parameters




### -param brush [in]

Type: <b>const <a href="https://msdn.microsoft.com/37cfc0f8-8e17-4944-85fc-cc80ebff13df">Brush</a>*</b>

Pointer to a brush that is used to paint the interior of the ellipse. 


### -param x [in]

Type: <b>REAL</b>

Real number that specifies the x-coordinate of the upper-left corner of the rectangle that specifies the boundaries of the ellipse. 


### -param y [in]

Type: <b>REAL</b>

Real number that specifies the y-coordinate of the upper-left corner of the rectangle that specifies the boundaries of the ellipse. 


### -param width [in]

Type: <b>REAL</b>

Real number that specifies the width of the rectangle that specifies the boundaries of the ellipse. 


### -param height [in]

Type: <b>REAL</b>

Real number that specifies the height of the rectangle that specifies the boundaries of the ellipse. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/889558d5-9181-43ff-b862-e92966324208">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/7e874710-3cd3-42c8-bd2f-8a779b19ba59">Graphics</a>



<a href="https://msdn.microsoft.com/8d5c8780-f03c-40b2-b237-e40121e3d6f6">SolidBrush</a>



<a href="https://msdn.microsoft.com/8ccf2c4a-6f99-465f-8adf-0f7fcd002f79">Using a Brush to Fill Shapes</a>
 

 

