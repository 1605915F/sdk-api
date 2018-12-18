---
UID: NF:gdiplusgraphics.Graphics.DrawCurve(IN const Pen,IN const PointF,IN INT,IN INT,IN INT,IN REAL)
title: Graphics::DrawCurve(IN const Pen,IN const PointF,IN INT,IN INT,IN INT,IN REAL)
author: windows-sdk-content
description: The Graphics::DrawCurve method draws a cardinal spline.
old-location: gdiplus\_gdiplus_CLASS_Graphics_DrawCurve_Pen_pen_PointF_points_INT_count_INT_offset_INT_numberOfSegments_RE.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\graphicsdrawcurvemethods\drawcurve_65penpen_pointfpoints_intcount_intoffset.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DrawCurve, DrawCurve method [GDI+], DrawCurve method [GDI+],Graphics class, Graphics class [GDI+],DrawCurve method, Graphics.DrawCurve, Graphics.DrawCurve(IN const Pen,IN const PointF,IN INT,IN INT,IN INT,IN REAL), Graphics.DrawCurve(const Pen*,const PointF*,INT,INT,INT,REAL), Graphics::DrawCurve, Graphics::DrawCurve(IN const Pen,IN const PointF,IN INT,IN INT,IN INT,IN REAL), _gdiplus_CLASS_Graphics_DrawCurve_Pen_pen_PointF_points_INT_count_INT_offset_INT_numberOfSegments_RE, gdiplus._gdiplus_CLASS_Graphics_DrawCurve_Pen_pen_PointF_points_INT_count_INT_offset_INT_numberOfSegments_RE
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
 - Graphics.DrawCurve
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Graphics::DrawCurve(IN const Pen,IN const PointF,IN INT,IN INT,IN INT,IN REAL)


## -description


The <b>Graphics::DrawCurve</b> method draws a cardinal spline.


## -parameters




### -param pen [in]

Type: <b>const <a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a>*</b>

Pointer to a pen that is used to draw the cardinal spline. 


### -param points [in]

Type: <b>const <a href="https://msdn.microsoft.com/2d357844-19a8-4ada-ba1e-685fea2e65ce">PointF</a>*</b>

Pointer to an array of 
					<a href="https://msdn.microsoft.com/2d357844-19a8-4ada-ba1e-685fea2e65ce">PointF</a> objects that specify the coordinates that the cardinal spline passes through. 


### -param count [in]

Type: <b>INT</b>

Integer that specifies the number of elements in the 
					<i>points</i> array. 


### -param offset [in]

Type: <b>INT</b>

Integer that specifies the element in the 
					<i>points</i> array that specifies the point at which the cardinal spline begins. 


### -param numberOfSegments [in]

Type: <b>INT</b>

Integer that specifies the number of segments in the cardinal spline. 


### -param tension [in]

Type: <b>REAL</b>

Real number that specifies how tightly the curve bends through the coordinates of the cardinal spline. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -remarks



A segment is defined as a curve that connects two consecutive points in the cardinal spline. The ending point of each segment is the starting point for the next. The 
				<i>numberOfSegments</i> parameter must not be greater than the 
				<i>count</i> parameter minus the 
				<i>offset</i> parameter plus one.


#### Examples



The following example draws a cardinal spline.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_DrawCurve5(HDC hdc)
{
   Graphics graphics(hdc);

   // Define a Pen object and an array of PointF objects.
   Pen greenPen(Color::Green, 3);
   PointF point1(100.0f, 100.0f);
   PointF point2(200.0f, 50.0f);
   PointF point3(400.0f, 10.0f);
   PointF point4(500.0f, 100.0f);

   PointF curvePoints[4] = {
   point1,
   point2,
   point3,
   point4};

   PointF* pcurvePoints = curvePoints;

   // Specify offset, number of segments to draw, and tension.
   int offset = 1;
   int segments = 2;
   REAL tension = 1.0f;

   // Draw the curve.
   graphics.DrawCurve(&amp;greenPen, curvePoints, 4, offset, segments, tension);

   //Draw the points in the curve.
   SolidBrush redBrush(Color::Red);
   graphics.FillEllipse(&amp;redBrush, Rect(95, 95, 10, 10));
   graphics.FillEllipse(&amp;redBrush, Rect(195, 45, 10, 10));
   graphics.FillEllipse(&amp;redBrush, Rect(395, 5, 10, 10));
   graphics.FillEllipse(&amp;redBrush, Rect(495, 95, 10, 10));
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/4fc62f00-7006-4ade-bfcc-091a3a97d889">Cardinal Splines</a>



<a href="https://msdn.microsoft.com/366c883b-0acf-4c2d-8ecd-18baa1c75b76">DrawClosedCurve Methods</a>



<a href="https://msdn.microsoft.com/0bb84f55-18d0-4a4c-bc5b-7803aa807954">Drawing Cardinal Splines</a>



<a href="https://msdn.microsoft.com/7e874710-3cd3-42c8-bd2f-8a779b19ba59">Graphics</a>



<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a>



<a href="https://msdn.microsoft.com/8bf4d566-b061-4102-8307-218431e286f8">Point</a>
 

 

