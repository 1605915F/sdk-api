---
UID: NF:gdiplusgraphics.Graphics.ScaleTransform
title: Graphics::ScaleTransform (gdiplusgraphics.h)
author: windows-sdk-content
description: The Graphics::ScaleTransform method updates this Graphics object's world transformation matrix with the product of itself and a scaling matrix.
old-location: gdiplus\_gdiplus_CLASS_Graphics_ScaleTransform_sx_sy_order_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\scaletransform.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Graphics class [GDI+],ScaleTransform method, Graphics.ScaleTransform, Graphics::ScaleTransform, ScaleTransform, ScaleTransform method [GDI+], ScaleTransform method [GDI+],Graphics class, _gdiplus_CLASS_Graphics_ScaleTransform_sx_sy_order_, gdiplus._gdiplus_CLASS_Graphics_ScaleTransform_sx_sy_order_
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
 - Graphics.ScaleTransform
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
ms.custom: 19H1
---

# Graphics::ScaleTransform


## -description


The <b>Graphics::ScaleTransform</b> method updates this <a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a> object's world transformation matrix with the product of itself and a scaling matrix.


## -parameters




### -param sx [in]

Type: <b>REAL</b>

Real number that specifies the horizontal scaling factor in the scaling matrix. 


### -param sy [in]

Type: <b>REAL</b>

Real number that specifies the vertical scaling factor in the scaling matrix. 


### -param order [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a></b>

Optional. Element of the <a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a> enumeration that specifies the order of multiplication. MatrixOrderPrepend specifies that the scaling matrix is on the left, and MatrixOrderAppend specifies that the scaling matrix is on the right. The default value is MatrixOrderPrepend. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms536332(v=VS.85).aspx">Coordinate Systems and Transformations</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535729(v=VS.85).aspx">Graphics::GetTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535800(v=VS.85).aspx">Graphics::MultiplyTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535803(v=VS.85).aspx">Graphics::ResetTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535805(v=VS.85).aspx">Graphics::RotateTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535820(v=VS.85).aspx">Graphics::TranslateTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534475(v=VS.85).aspx">Matrix</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533810(v=VS.85).aspx">Transformations</a>
 

 

