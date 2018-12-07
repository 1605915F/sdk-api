---
UID: NF:msinkaut.IInkDrawingAttributes.Clone
title: IInkDrawingAttributes::Clone
author: windows-sdk-content
description: Creates a duplicate InkDrawingAttributes object.
old-location: tablet\inkdrawingattributes_clone.htm
tech.root: tablet
ms.assetid: 97facd95-af49-459e-82fc-12534d466786
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Clone, Clone method [Tablet PC], Clone method [Tablet PC],IInkDrawingAttributes interface, IInkDrawingAttributes interface [Tablet PC],Clone method, IInkDrawingAttributes.Clone, IInkDrawingAttributes::Clone, f3ec6b42-2b5d-459e-ba09-88c27b125c40, msinkaut/IInkDrawingAttributes::Clone, tablet.inkdrawingattributes_clone
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IInkDrawingAttributes.Clone
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInkDrawingAttributes::Clone


## -description



Creates a duplicate <a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes</a> object.




## -parameters




### -param DrawingAttributes [out, retval]

When this method returns, contains a pointer to the newly created <a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes</a> object.


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
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Cannot allocate memory to complete the operation.

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
<dt><b>REGDB_CLASSNOTREG</b></dt>
</dl>
</td>
<td width="60%">
The <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a> object was not registered.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
Unexpected parameter or property type.

</td>
</tr>
</table>
 




## -remarks



The <a href="https://msdn.microsoft.com/f3ec6b42-2b5d-459e-ba09-88c27b125c40">Clone</a> method is defined for the <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a>, <a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes</a>, and <a href="https://msdn.microsoft.com/2b39fd32-831d-4606-8600-b52aaa7ed882">InkRecognizerContext</a> objects. The <b>Clone</b> method returns an exact copy of the original object.

In most scenarios, the duplicate object is an exact copy of the original object, but no relation between the two objects exists. See the remarks section of this topic for details on exceptions to this.


<a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes</a> object: Typically, you clone a master copy of the drawing attributes, modify one or more of the attributes, and call the <a href="https://msdn.microsoft.com/b249edd9-dfa4-4538-9764-a4365f9df527">ModifyDrawingAttributes</a> method to use the modified drawing attributes.




## -see-also




<a href="https://msdn.microsoft.com/3399219f-96a5-4c66-8e41-89927ea1020d">Dirty Property</a>



<a href="https://msdn.microsoft.com/47106C55-FA03-4996-BCFA-D00A51AF55EE">IInkDrawingAttributes</a>



<a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttribute Class</a>



<a href="https://msdn.microsoft.com/b249edd9-dfa4-4538-9764-a4365f9df527">ModifyDrawingAttributes Method</a>
 

 

