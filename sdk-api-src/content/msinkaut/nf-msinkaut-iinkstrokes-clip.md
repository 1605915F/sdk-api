---
UID: NF:msinkaut.IInkStrokes.Clip
title: IInkStrokes::Clip (msinkaut.h)
author: windows-sdk-content
description: Removes portions of an IInkStrokeDisp object or InkStrokes collection that are outside a rectangle.
old-location: tablet\inkstrokes_clip.htm
tech.root: tablet
ms.assetid: ef434bcc-610c-449d-90d4-b3f897408f34
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Clip, Clip method [Tablet PC], Clip method [Tablet PC],IInkStrokes interface, IInkStrokes interface [Tablet PC],Clip method, IInkStrokes.Clip, IInkStrokes::Clip, d3733613-fc8e-41f2-9172-07b61fc133dd, msinkaut/IInkStrokes::Clip, tablet.inkstrokes_clip
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
 - IInkStrokes.Clip
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IInkStrokes::Clip


## -description



Removes portions of an <a href="https://msdn.microsoft.com/b18464ba-feb6-4bb5-9fcf-82feff9bcce4">IInkStrokeDisp</a> object or <a href="https://msdn.microsoft.com/c7fb921c-0bd2-48aa-b092-ab1fb08c0697">InkStrokes</a> collection that are outside a rectangle.




## -parameters




### -param Rectangle [in]

Specifies the rectangle outside of which the stroke or strokes are clipped. The rectangle is specified in ink space coordinates.


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
<dt><b>REGDB_CLASSNOTREG</b></dt>
</dl>
</td>
<td width="60%">
The <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a> object is not registered.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid clip rectangle.

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
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unspecified error occurred.

</td>
</tr>
</table>
 




## -remarks



For an <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a> object, all strokes intersected by the rectangle are split at the intersection points. All portions of strokes outside the rectangle are removed from the <b>InkDisp</b> object. The method may add new points to a stroke at the point where the stroke intersects the rectangle. After you call the <a href="https://msdn.microsoft.com/d3733613-fc8e-41f2-9172-07b61fc133dd">Clip</a> method on an <b>InkDisp</b> object, the IDs of the strokes in the <b>InkDisp</b> object's strokes collection are guaranteed to be unique, but not guaranteed to preserve other information.

This method does not take the pen width into account when clipping. It clips only the actual ink or stroke data.

For an <a href="https://msdn.microsoft.com/b18464ba-feb6-4bb5-9fcf-82feff9bcce4">IInkStrokeDisp</a> object or <a href="https://msdn.microsoft.com/c7fb921c-0bd2-48aa-b092-ab1fb08c0697">InkStrokes</a> collection, the <a href="https://msdn.microsoft.com/d3733613-fc8e-41f2-9172-07b61fc133dd">Clip</a> method updates the parent <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a> object. Whenever ink is removed from an <b>InkDisp</b> object, any <b>IInkStrokeDisp</b> objects or InkStrokes collections defined for that <b>InkDisp</b> object may be invalidated.

For more information on ink data, see <a href="https://msdn.microsoft.com/5a8c370e-79cb-47f0-a7b3-a631874ad757">Ink Data</a>.




## -see-also




<a href="https://msdn.microsoft.com/401c4f62-a406-49ac-9911-91f815cde9c8">HitTest(Rectangle, Single) Method</a>



<a href="https://msdn.microsoft.com/en-us/library/Mt846806(v=VS.85).aspx">IInkStrokes</a>



<a href="https://msdn.microsoft.com/78e6c29c-0f43-46a5-9d30-948de5f369c8">InkRectangle Class</a>



<a href="https://msdn.microsoft.com/c7fb921c-0bd2-48aa-b092-ab1fb08c0697">InkStrokes Collection</a>
 

 

