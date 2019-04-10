---
UID: NF:gdiplusgraphics.Graphics.GetTransform
title: Graphics::GetTransform (gdiplusgraphics.h)
author: windows-sdk-content
description: The Graphics::GetTransform method gets the world transformation matrix of this Graphics object.
old-location: gdiplus\_gdiplus_CLASS_Graphics_GetTransform_matrix_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\gettransform.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetTransform, GetTransform method [GDI+], GetTransform method [GDI+],Graphics class, Graphics class [GDI+],GetTransform method, Graphics.GetTransform, Graphics::GetTransform, _gdiplus_CLASS_Graphics_GetTransform_matrix_, gdiplus._gdiplus_CLASS_Graphics_GetTransform_matrix_
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
 - Graphics.GetTransform
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Graphics::GetTransform


## -description


The <b>Graphics::GetTransform</b> method gets the world transformation matrix of this 
			<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a> object.


## -parameters




### -param matrix [out]

Type: <b>Matrix*</b>

Pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms534475(v=VS.85).aspx">Matrix</a> object that receives the transformation matrix. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms536332(v=VS.85).aspx">Coordinate Systems and Transformations</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535800(v=VS.85).aspx">Graphics::MultiplyTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535803(v=VS.85).aspx">Graphics::ResetTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535805(v=VS.85).aspx">Graphics::RotateTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535807(v=VS.85).aspx">Graphics::ScaleTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535818(v=VS.85).aspx">Graphics::SetTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535819(v=VS.85).aspx">Graphics::TransformPoints</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535820(v=VS.85).aspx">Graphics::TranslateTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534475(v=VS.85).aspx">Matrix</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533810(v=VS.85).aspx">Transformations</a>
 

 

