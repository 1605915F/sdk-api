---
UID: NF:msinkaut.IInkRenderer.SetObjectTransform
title: IInkRenderer::SetObjectTransform
author: windows-sdk-content
description: Sets the InkTransform object that represents the object transform that is used to render ink.
old-location: tablet\inkrenderer_setobjecttransform.htm
tech.root: tablet
ms.assetid: 8d0cbc97-d9a2-4b6c-8e92-55237cef6523
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 8d0cbc97-d9a2-4b6c-8e92-55237cef6523, IInkRenderer interface [Tablet PC],SetObjectTransform method, IInkRenderer.SetObjectTransform, IInkRenderer::SetObjectTransform, SetObjectTransform, SetObjectTransform method [Tablet PC], SetObjectTransform method [Tablet PC],IInkRenderer interface, msinkaut/IInkRenderer::SetObjectTransform, tablet.inkrenderer_setobjecttransform
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
 - IInkRenderer.SetObjectTransform
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInkRenderer::SetObjectTransform


## -description



Sets the <a href="https://msdn.microsoft.com/79abff2e-d1d3-4a32-9ac2-f46c1b21f742">InkTransform</a> object that represents the object transform that is used to render ink.




## -parameters




### -param ObjectTransform [in]

The <a href="https://msdn.microsoft.com/79abff2e-d1d3-4a32-9ac2-f46c1b21f742">InkTransform</a> object that represents the geometric transformation - rotation, scaling, shear, and reflection - values to use to transform the stroke coordinates within the ink space.

A <b>NULL</b> value for the <i>objectTransform</i> parameter correlates to the identity transform.


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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
<i>objectTransform</i> does not point to a compatible <a href="https://msdn.microsoft.com/79abff2e-d1d3-4a32-9ac2-f46c1b21f742">InkTransform</a> object.

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
</table>
 




## -remarks



The transformation applies to the points, but not the pen width.

Object transformation occurs before view transformation.

It is problematic to call this method in response to SENT message.  Test whether you are processing a SENT message
			  by calling <a href="https://msdn.microsoft.com/en-us/library/ms644942(v=VS.85).aspx">InSendMesssageEx</a> and then POST the message to yourself if the message was SENT.




## -see-also




<a href="https://msdn.microsoft.com/11195fa1-ca59-4da6-8454-6209c75ccc67">GetObjectTransform Method</a>



<a href="https://msdn.microsoft.com/8a4d768d-09b6-45e1-b412-e267d92cc3ef">GetViewTransform Method</a>



<a href="https://msdn.microsoft.com/2AB56616-3F67-4428-8A99-FCE733A5FDBF">IInkRenderer</a>



<a href="https://msdn.microsoft.com/66ec7cab-bfc2-4934-93a4-0ab9cb8c96e7">InkRenderer Class</a>



<a href="https://msdn.microsoft.com/b1850d41-4523-4a2b-a7ae-6b85d1ae9a97">SetViewTransform Method</a>
 

 

