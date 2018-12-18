---
UID: NF:gdipluspath.GraphicsPath.AddClosedCurve(IN const Point,IN INT,IN REAL)
title: GraphicsPath::AddClosedCurve(IN const Point,IN INT,IN REAL)
author: windows-sdk-content
description: The GraphicsPath::AddClosedCurve method adds a closed cardinal spline to this path.
old-location: gdiplus\_gdiplus_CLASS_GraphicsPath_AddClosedCurve_Point_points_INT_count_REAL_tension_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicspathclass\graphicspathmethods\graphicspathaddclosedcurvemethods\addclosedcurve_5pointpoints_intcount_realtension.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddClosedCurve, AddClosedCurve method [GDI+], AddClosedCurve method [GDI+],GraphicsPath class, GraphicsPath class [GDI+],AddClosedCurve method, GraphicsPath.AddClosedCurve, GraphicsPath.AddClosedCurve(IN const Point,IN INT,IN REAL), GraphicsPath.AddClosedCurve(const Point*,INT,REAL), GraphicsPath::AddClosedCurve, GraphicsPath::AddClosedCurve(IN const Point,IN INT,IN REAL), _gdiplus_CLASS_GraphicsPath_AddClosedCurve_Point_points_INT_count_REAL_tension_, gdiplus._gdiplus_CLASS_GraphicsPath_AddClosedCurve_Point_points_INT_count_REAL_tension_
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
 - GraphicsPath.AddClosedCurve
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# GraphicsPath::AddClosedCurve(IN const Point,IN INT,IN REAL)


## -description


The <b>GraphicsPath::AddClosedCurve</b> method adds a closed cardinal spline to this path.


## -parameters




### -param points [in]

Type: <b>const <a href="https://msdn.microsoft.com/8bf4d566-b061-4102-8307-218431e286f8">Point</a>*</b>

Pointer to an array of points that define the cardinal spline. The cardinal spline is a curve that passes through each point in the array. 


### -param count [in]

Type: <b>INT</b>

Integer that specifies the number of elements in the
					<i>points</i> array. 


### -param tension [in]

Type: <b>REAL</b>

Nonnegative real number that controls the length of the curve and how the curve bends. A value of 0 specifies that the spline is a sequence of straight lines. As the value increases, the curve becomes fuller. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -remarks



You should keep a copy of the <i>points</i> array if those points will be needed later. The <a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a> object does not store the points passed to the <b>GraphicsPath::AddClosedCurve</b> method; instead, it converts the cardinal spline to a sequence of Bézier splines and stores the points that define those Bézier splines. You cannot retrieve the original array of points from the <b>GraphicsPath</b> object.


#### Examples



The following example creates a <a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a> object <i>path</i>, adds a closed cardinal spline to <i>path</i>, and then draws <i>path</i>. The tension is set to 1.0.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_AddClosedCurve(HDC hdc)
{
   Graphics graphics(hdc); 

   Point pts[] = {Point(50,50),
                  Point(60,20),
                  Point(70,100),
                  Point(80,50)};

   GraphicsPath path;
   path.AddClosedCurve(pts, 4, 1.0f);

   // Draw the path.
   Pen pen(Color(255, 255, 0, 0));
   graphics.DrawPath(&amp;pen, &amp;path);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/1c4f3d1b-1fdb-4fde-8f69-bcfac1a33663">AddBezier Methods</a>



<a href="https://msdn.microsoft.com/fb754409-1867-41bd-a9d3-952e393490f8">AddBeziers Methods</a>



<a href="https://msdn.microsoft.com/5a633a04-1de4-43f5-a898-d30245567e5d">AddClosedCurve Methods</a>



<a href="https://msdn.microsoft.com/81f43f7e-a383-44f7-a3bd-2969d541b616">AddCurve Methods</a>



<a href="https://msdn.microsoft.com/4fc62f00-7006-4ade-bfcc-091a3a97d889">Cardinal Splines</a>



<a href="https://msdn.microsoft.com/816a5845-ca03-46c6-bdda-e6a7d02ff614">Clipping with a Region</a>



<a href="https://msdn.microsoft.com/dbfe8cea-bd9e-43ad-85c8-37cce3ef97a4">Constructing and Drawing Paths</a>



<a href="https://msdn.microsoft.com/f6a8085c-3d6a-494f-a1ee-5fa96efb1aae">Creating a Path Gradient</a>



<a href="https://msdn.microsoft.com/0bb84f55-18d0-4a4c-bc5b-7803aa807954">Drawing Cardinal Splines</a>



<a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>



<a href="https://msdn.microsoft.com/88fea2ec-7b53-44bb-841d-486c5c879c68">Paths</a>



<a href="https://msdn.microsoft.com/8bf4d566-b061-4102-8307-218431e286f8">Point</a>
 

 

