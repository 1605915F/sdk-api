---
UID: NF:msinkaut.IInkLineInfo.SetFormat
title: IInkLineInfo::SetFormat (msinkaut.h)
author: windows-sdk-content
description: Specifies the display properties to set on the text ink object (tInk).
old-location: tablet\iinklineinfo_setformat.htm
tech.root: tablet
ms.assetid: 42e16e86-fc90-4089-9ae0-9a896cbeaccc
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 42e16e86-fc90-4089-9ae0-9a896cbeaccc, IInkLineInfo interface [Tablet PC],SetFormat method, IInkLineInfo.SetFormat, IInkLineInfo::SetFormat, SetFormat, SetFormat method [Tablet PC], SetFormat method [Tablet PC],IInkLineInfo interface, msinkaut/IInkLineInfo::SetFormat, tablet.iinklineinfo_setformat
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
 - IInkLineInfo.SetFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IInkLineInfo::SetFormat


## -description



Specifies the display properties to set on the text ink object (tInk).




## -parameters




### -param pim [in]

A pointer to an <a href="https://msdn.microsoft.com/27d56034-725d-4b05-9c43-6b3180d7411b">INKMETRIC</a> structure which contains the display properties to set on the text ink object.


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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>pim</i> parameter is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Could not complete the operation. The display properties are not changed.

</td>
</tr>
</table>
 




## -remarks



If the IMF_FONT_SELECTED_IN_HDC flag is set in the <i>pim</i> parameter, then the properties of the device context are applied to the ink; otherwise, the <a href="https://msdn.microsoft.com/27d56034-725d-4b05-9c43-6b3180d7411b">INKMETRIC</a> settings of the text ink object are applied.




## -see-also




<a href="https://msdn.microsoft.com/8f894963-7075-46f4-8809-82d1aa7e13e7">GetFormat Method</a>



<a href="https://msdn.microsoft.com/0082b7d3-61b2-478a-a6dd-ba59c20b7e1d">GetInkExtent Method</a>



<a href="https://msdn.microsoft.com/58774f49-6af2-4b81-bbd5-709eb694af2d">IInkLineInfo</a>



<a href="https://msdn.microsoft.com/27d56034-725d-4b05-9c43-6b3180d7411b">INKMETRIC Structure</a>
 

 

