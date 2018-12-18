---
UID: NF:gdiplustypes.Point.operator-sub
title: Point::operator-sub
author: windows-sdk-content
description: The Point::operator- method subtracts the X and Y data members of two Point objects.
old-location: gdiplus\_gdiplus_CLASS_Point_operator_opminus_point_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\pointclass\pointmethods\operator_52point.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Point class [GDI+],operator- method, Point.operator-, Point.operator-(const Point&), Point.operator-sub, Point::operator-, Point::operator-sub, _gdiplus_CLASS_Point_operator_opminus_point_, gdiplus._gdiplus_CLASS_Point_operator_opminus_point_, operator-, operator- method [GDI+], operator- method [GDI+],Point class
ms.topic: method
req.header: gdiplustypes.h
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
 - Point.operator-
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Point::operator-sub


## -description


The <b>Point::operator-</b> method subtracts the <b>X</b> and <b>Y</b> data members of two <a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a> objects.


## -parameters




### -param point [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a></b>

Reference to a <a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a> object whose <b>X</b> and <b>Y</b> data members are subtracted from the <b>X</b> and <b>Y</b> data members of this <b>Point</b> object. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a></b>
</strong>

This method returns a <a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a> object that is the difference of two <b>Point</b> objects.




## -remarks



This method overloads the subtraction operator for <a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a> objects. If A, B, and C are <b>Point</b> objects, the statement <b>C = A - B</b> is equivalent to <b>C = A.operator-(B)</b>.


#### Examples



The following example creates two <a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a> objects, then subtracts the second <b>Point</b> object from the first <b>Point</b> object and stores the result in a third <b>Point</b> object.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>Point point1(40, 10);
Point point2(-20, -30);

// Point3 now contains the coordinates (60, 40).
Point point3 = point1 - point2; </pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms534487(v=VS.85).aspx">Point</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535007(v=VS.85).aspx">Point::Equals</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535008(v=VS.85).aspx">Point::operator+</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534488(v=VS.85).aspx">PointF</a>
 

 

