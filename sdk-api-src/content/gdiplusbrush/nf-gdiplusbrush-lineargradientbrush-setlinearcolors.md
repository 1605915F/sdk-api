---
UID: NF:gdiplusbrush.LinearGradientBrush.SetLinearColors
title: LinearGradientBrush::SetLinearColors (gdiplusbrush.h)
author: windows-sdk-content
description: The LinearGradientBrush::SetLinearColors method sets the starting color and ending color of this linear gradient brush.
old-location: gdiplus\_gdiplus_CLASS_LinearGradientBrush_SetLinearColors_color1_color2_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\lineargradientbrushclass\lineargradientbrushmethods\setlinearcolors.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: LinearGradientBrush class [GDI+],SetLinearColors method, LinearGradientBrush.SetLinearColors, LinearGradientBrush::SetLinearColors, SetLinearColors, SetLinearColors method [GDI+], SetLinearColors method [GDI+],LinearGradientBrush class, _gdiplus_CLASS_LinearGradientBrush_SetLinearColors_color1_color2_, gdiplus._gdiplus_CLASS_LinearGradientBrush_SetLinearColors_color1_color2_
ms.topic: method
req.header: gdiplusbrush.h
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
 - LinearGradientBrush.SetLinearColors
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# LinearGradientBrush::SetLinearColors


## -description


The <b>LinearGradientBrush::SetLinearColors</b> method sets the starting color and ending color of this linear gradient brush.


## -parameters




### -param color1 [in]

Type: <b>const Color&amp;</b>

Reference to a <a href="https://msdn.microsoft.com/en-us/library/ms534427(v=VS.85).aspx">Color</a> object that specifies the color at the starting boundary line of this linear gradient brush. 


### -param color2 [in]

Type: <b>const Color&amp;</b>

Reference to a <a href="https://msdn.microsoft.com/en-us/library/ms534427(v=VS.85).aspx">Color</a> object that specifies the color at the ending boundary line of this linear gradient brush. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms536356(v=VS.85).aspx">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534427(v=VS.85).aspx">Color</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533914(v=VS.85).aspx">Creating a Linear Gradient</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533856(v=VS.85).aspx">Filling a Shape with a Color Gradient</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534473(v=VS.85).aspx">LinearGradientBrush</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535334(v=VS.85).aspx">LinearGradientBrush::GetLinearColors</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535346(v=VS.85).aspx">LinearGradientBrush::SetInterpolationColors</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a>
 

 

