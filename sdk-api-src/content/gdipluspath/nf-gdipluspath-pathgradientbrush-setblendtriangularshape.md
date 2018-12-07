---
UID: NF:gdipluspath.PathGradientBrush.SetBlendTriangularShape
title: PathGradientBrush::SetBlendTriangularShape
author: windows-sdk-content
description: The PathGradientBrush::SetBlendTriangularShape method sets the blend shape of this path gradient brush.
old-location: gdiplus\_gdiplus_CLASS_PathGradientBrush_SetBlendTriangularShape_focus_scale_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\pathgradientbrushclass\pathgradientbrushmethods\setblendtriangularshape_1focus_scale.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PathGradientBrush class [GDI+],SetBlendTriangularShape method, PathGradientBrush.SetBlendTriangularShape, PathGradientBrush::SetBlendTriangularShape, SetBlendTriangularShape, SetBlendTriangularShape method [GDI+], SetBlendTriangularShape method [GDI+],PathGradientBrush class, _gdiplus_CLASS_PathGradientBrush_SetBlendTriangularShape_focus_scale_, gdiplus._gdiplus_CLASS_PathGradientBrush_SetBlendTriangularShape_focus_scale_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdipluspath.h
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
 - PathGradientBrush.SetBlendTriangularShape
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# PathGradientBrush::SetBlendTriangularShape


## -description


The <b>PathGradientBrush::SetBlendTriangularShape</b> method sets the blend shape of this path gradient brush.


## -parameters




### -param focus [in]

Type: <b>REAL</b>

Real number that specifies where the center color will be at its highest intensity. This number must be in the range 0 through 1. 


### -param scale [in, optional]

Type: <b>REAL</b>

Optional. Real number that specifies the maximum intensity of center color that gets blended with the boundary color. This number must be in the range 0 through 1. The default value is 1. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -remarks



By default, as you move from the boundary of a path gradient to the center point, the color changes gradually from the boundary color to the center color. You can customize the positioning and blending of the boundary and center colors by calling the <b>PathGradientBrush::SetBlendTriangularShape</b> method.


#### Examples



The following example creates a 
						<a href="https://msdn.microsoft.com/en-us/library/ms534483(v=VS.85).aspx">PathGradientBrush</a>object based on an ellipse. The code calls the <b>PathGradientBrush::SetBlendTriangularShape</b> method of the 
						<b>PathGradientBrush</b>object, passing a focus of 0.2 and a scale of 0.7. Then the code uses the path gradient brush to paint a rectangle that contains the ellipse.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_SetBlendShape(HDC hdc)
{
   Graphics graphics(hdc);

   // Create a path that consists of a single ellipse.
   GraphicsPath path;
   path.AddEllipse(0, 0, 200, 100);

   // Use the path to construct a brush.
   PathGradientBrush pthGrBrush(&amp;path);

   // Set the color at the center of the path to red.
   pthGrBrush.SetCenterColor(Color(255, 255, 0, 0));

   // Set the color along the entire boundary of the path to blue.
   Color colors[] = {Color(255, 0, 0, 255)};
   INT count = 1;
   pthGrBrush.SetSurroundColors(colors, &amp;count);

   pthGrBrush.SetBlendTriangularShape(0.2f, 0.7f);

   // The color is blue on the boundary and at the center.
   // At points that are 20 percent of the way from the boundary to the
   // center, the color is 70 percent red and 30 percent blue.

   graphics.FillRectangle(&amp;pthGrBrush, 0, 0, 300, 300); 
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms536356(v=VS.85).aspx">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534427(v=VS.85).aspx">Color</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533917(v=VS.85).aspx">Creating a Path Gradient</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533856(v=VS.85).aspx">Filling a Shape with a Color Gradient</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534456(v=VS.85).aspx">GraphicsPath</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534483(v=VS.85).aspx">PathGradientBrush</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535063(v=VS.85).aspx">PathGradientBrush::GetBlend</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535062(v=VS.85).aspx">PathGradientBrush::GetBlendCount</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535084(v=VS.85).aspx">PathGradientBrush::SetBlend</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535082(v=VS.85).aspx">PathGradientBrush::SetBlendBellShape</a>
 

 

