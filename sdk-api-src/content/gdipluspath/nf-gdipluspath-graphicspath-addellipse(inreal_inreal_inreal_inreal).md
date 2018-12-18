---
UID: NF:gdipluspath.GraphicsPath.AddEllipse(IN REAL,IN REAL,IN REAL,IN REAL)
title: GraphicsPath::AddEllipse(IN REAL,IN REAL,IN REAL,IN REAL)
author: windows-sdk-content
description: The GraphicsPath::AddEllipse method adds an ellipse to this path.
old-location: gdiplus\_gdiplus_CLASS_GraphicsPath_AddEllipse_REAL_x_REAL_y_REAL_width_REAL_height_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicspathclass\graphicspathmethods\graphicspathaddellipsemethods\addellipse_69realx_realy_realwidth_realheight.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddEllipse, AddEllipse method [GDI+], AddEllipse method [GDI+],GraphicsPath class, GraphicsPath class [GDI+],AddEllipse method, GraphicsPath.AddEllipse, GraphicsPath.AddEllipse(IN REAL,IN REAL,IN REAL,IN REAL), GraphicsPath.AddEllipse(REAL,REAL,REAL,REAL), GraphicsPath::AddEllipse, GraphicsPath::AddEllipse(IN REAL,IN REAL,IN REAL,IN REAL), _gdiplus_CLASS_GraphicsPath_AddEllipse_REAL_x_REAL_y_REAL_width_REAL_height_, gdiplus._gdiplus_CLASS_GraphicsPath_AddEllipse_REAL_x_REAL_y_REAL_width_REAL_height_
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
 - GraphicsPath.AddEllipse
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# GraphicsPath::AddEllipse(IN REAL,IN REAL,IN REAL,IN REAL)


## -description


The <b>GraphicsPath::AddEllipse</b> method adds an ellipse to this path.


## -parameters




### -param x [in]

Type: <b>REAL</b>

Real number that specifies the x-coordinate of the upper-left corner of the bounding rectangle for the ellipse. 


### -param y [in]

Type: <b>REAL</b>

Real number that specifies the y-coordinate of the upper-left corner of the bounding rectangle for the ellipse. 


### -param width [in]

Type: <b>REAL</b>

Real number that specifies the width of the bounding rectangle for the ellipse. 


### -param height [in]

Type: <b>REAL</b>

Real number that specifies the height of the bounding rectangle for the ellipse. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -remarks



A <a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a> object stores an ellipse as a sequence of four connected Bézier splines. The <b>GraphicsPath</b> object does not store the upper-left corner, width, and height of the ellipse's bounding rectangle.


#### Examples



The following example creates a <a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a> object <i>path</i>, adds an ellipse to <i>path</i>, and then draws <i>path</i>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_AddEllipse(HDC hdc)
{
   Graphics graphics(hdc); 

   GraphicsPath path;
   path.AddEllipse(20.0f, 20.0f, 200.0f, 100.0f);

   // Draw the path.
   Pen pen(Color(255, 255, 0, 0));
   graphics.DrawPath(&amp;pen, &amp;path);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/54171039-4cb9-4898-a656-b7a9df4b18f6">AddArc Methods</a>



<a href="https://msdn.microsoft.com/39074cd8-267d-485a-8175-d0a25dcf9097">AddEllipse Methods</a>



<a href="https://msdn.microsoft.com/816a5845-ca03-46c6-bdda-e6a7d02ff614">Clipping with a Region</a>



<a href="https://msdn.microsoft.com/dbfe8cea-bd9e-43ad-85c8-37cce3ef97a4">Constructing and Drawing Paths</a>



<a href="https://msdn.microsoft.com/f6a8085c-3d6a-494f-a1ee-5fa96efb1aae">Creating a Path Gradient</a>



<a href="https://msdn.microsoft.com/45e80501-4d64-480b-a7c7-3af52c00a0aa">Ellipses and Arcs</a>



<a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>



<a href="https://msdn.microsoft.com/88fea2ec-7b53-44bb-841d-486c5c879c68">Paths</a>
 

 

