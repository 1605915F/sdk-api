---
UID: NF:msinkaut.IInkDisp.HitTestWithLasso
title: IInkDisp::HitTestWithLasso
author: windows-sdk-content
description: Retrieves the strokes within a polyline selection area.
old-location: tablet\inkdisp_hittest_point____single.htm
tech.root: tablet
ms.assetid: fe88410d-e3e7-4899-b6fe-04e6eed98bbb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: HitTestWithLasso, HitTestWithLasso method [Tablet PC], HitTestWithLasso method [Tablet PC],IInkDisp interface, IInkDisp interface [Tablet PC],HitTestWithLasso method, IInkDisp.HitTestWithLasso, IInkDisp::HitTestWithLasso, fe88410d-e3e7-4899-b6fe-04e6eed98bbb, msinkaut/IInkDisp::HitTestWithLasso, tablet.inkdisp_hittest_point____single
ms.topic: method
req.header: msinkaut.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: InkObj.dll
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - InkObj.dll
 - InkObj.dll.dll
api_name:
 - IInkDisp.HitTestWithLasso
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInkDisp::HitTestWithLasso


## -description


Retrieves the strokes within a polyline selection area.
        


## -parameters




### -param Points [in]

The points that are used in the selection tool to select the strokes. The selection area is the area inside the selection boundary in which the boundary first intersects itself. If the boundary does not intersect itself, the method adds a point to the end of the array to create a straight line from the first point to the last point. If the boundary is a straight line (no area within the selection boundary), no strokes are selected.

For more information about the VARIANT structure, see <a href="https://msdn.microsoft.com/fa43fad9-804c-42d9-9717-6686d5f98ed8">Using the COM Library</a>.


### -param IntersectPercent [in]

The percentage of stroke points that must be contained within the selection tool to include the stroke in the resulting collection of strokes. If zero (<code>0</code>), all strokes that are contained within or intersected by the selection tool are included in the resulting collection of strokes. If 100, only strokes fully contained in the selection tool are included in the collection. Strokes that intersect the selection tool are included in the collection if the percentage of points in those strokes contained within the selection tool is greater than or equal to the <i>percentIntersect</i> percentage. Fractional percentages are rounded up.


### -param LassoPoints [in, out, optional]

Optional. Retrieves the specific portion of the selection tool that is used for the selection. Because a user can draw many different types of selection tools, some of which overlap multiple times, this can be useful for illustrating which portion of the selection tool was used for selection. The default value is a <b>NULL</b> pointer, which means no information is returned.

For more information about the VARIANT structure, see <a href="https://msdn.microsoft.com/fa43fad9-804c-42d9-9717-6686d5f98ed8">Using the COM Library</a>.


### -param Strokes [out, retval]

When this method returns, contains a pointer to the collection of strokes that makes up the ink.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
A parameter contained an invalid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INK_EXCEPTION</b></dt>
</dl>
</td>
<td width="60%">
An exception occurred inside the method.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid display handle.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Cannot allocate memory operation.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/2025f728-cb08-4285-8584-c9ad537e58f2">HitTest(Point, Single) Method</a>



<a href="https://msdn.microsoft.com/401c4f62-a406-49ac-9911-91f815cde9c8">HitTest(Rectangle, Single) Method</a>



<a href="https://msdn.microsoft.com/en-us/library/Mt846797(v=VS.85).aspx">IInkDisp</a>



<a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp Class</a>



<a href="https://msdn.microsoft.com/c7fb921c-0bd2-48aa-b092-ab1fb08c0697">InkStrokes Collection</a>
 

 

