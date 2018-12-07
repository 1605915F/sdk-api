---
UID: NF:ole.OleDraw
title: OleDraw function
author: windows-sdk-content
description: Enables drawing objects more easily. You can use it instead of calling IViewObject::Draw directly.
old-location: com\oledraw.htm
tech.root: com
ms.assetid: c45c6746-59ea-43bb-9f2b-2182d7a3fc7a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OleDraw, OleDraw function [COM], _ole_OleDraw, com.oledraw, ole/OleDraw
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: ole.h
req.include-header: Ole2.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
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
req.lib: Ole32.lib
req.dll: Ole32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Ole32.dll
 - ext-ms-win-com-ole32-l1-1-3.dll
 - Ext-MS-Win-Com-Ole32-L1-1-4.dll
api_name:
 - OleDraw
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# OleDraw function


## -description


Enables drawing objects more easily. You can use it instead of calling <a href="https://msdn.microsoft.com/913593ff-07fe-44bd-88dc-8e58da82089b">IViewObject::Draw</a> directly.


## -parameters




### -param arg1

TBD


### -param arg2

TBD


### -param arg3

TBD


### -param arg4

TBD


### -param arg5

TBD




#### - dwAspect [in]

How the object is to be represented. Representations include content, an icon, a thumbnail, or a printed document. Possible values are taken from the <a href="https://msdn.microsoft.com/a2b729c8-7091-4520-93cd-c44468ba0274">DVASPECT</a> enumeration.


#### - hdcDraw [in]

Device context on which to draw. Cannot be a metafile device context.


#### - lprcBounds [in]

Pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure specifying the rectangle in which the object should be drawn. This parameter is converted to a <a href="https://msdn.microsoft.com/47a89d2d-4733-47be-91c1-450845e78075">RECTL</a> structure and passed to <a href="https://msdn.microsoft.com/913593ff-07fe-44bd-88dc-8e58da82089b">IViewObject::Draw</a>.


#### - pUnknown [in]

Pointer to the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface on the view object that is to be drawn.


## -returns



This function returns S_OK on success. Other possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>OLE_E_BLANK</b></dt>
</dl>
</td>
<td width="60%">
No data to draw from.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_ABORT</b></dt>
</dl>
</td>
<td width="60%">
The draw operation was aborted.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>VIEW_E_DRAW</b></dt>
</dl>
</td>
<td width="60%">
No data to draw from.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>OLE_E_INVALIDRECT</b></dt>
</dl>
</td>
<td width="60%">
The rectangle is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG </b></dt>
</dl>
</td>
<td width="60%">
One or more parameters are invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory for the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DV_E_NOIVIEWOBJECT</b></dt>
</dl>
</td>
<td width="60%">
The object doesn't support the <a href="https://msdn.microsoft.com/4310c987-3542-4a59-a6fb-951143001741">IViewObject</a> interface.

</td>
</tr>
</table>
 




## -remarks



The OleDraw helper function calls the <a href="https://msdn.microsoft.com/54d5ff80-18db-43f2-b636-f93ac053146d">QueryInterface</a> method for the object specified (pUnk), asking for an <a href="https://msdn.microsoft.com/4310c987-3542-4a59-a6fb-951143001741">IViewObject</a> interface on that object. Then, <b>OleDraw</b> converts the <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure to a <a href="https://msdn.microsoft.com/47a89d2d-4733-47be-91c1-450845e78075">RECTL</a> structure, and calls <a href="https://msdn.microsoft.com/913593ff-07fe-44bd-88dc-8e58da82089b">IViewObject::Draw</a> as follows:

<pre class="syntax" xml:space="preserve"><code>lpViewObj-&gt;Draw(dwAspect,-1,0,0,0,hdcDraw,&amp;rectl,0,0,0);</code></pre>
Do not use this function to draw into a metafile because it does not specify the parameter required for drawing into metafiles.




## -see-also




<a href="https://msdn.microsoft.com/913593ff-07fe-44bd-88dc-8e58da82089b">IViewObject::Draw</a>
 

 

