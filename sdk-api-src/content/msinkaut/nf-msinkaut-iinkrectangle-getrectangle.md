---
UID: NF:msinkaut.IInkRectangle.GetRectangle
title: IInkRectangle::GetRectangle
author: windows-sdk-content
description: Gets the elements of the InkRectangle object in a single call.
old-location: tablet\inkrectangle_getrectangle.htm
tech.root: tablet
ms.assetid: 78efcd28-7095-49f7-b660-9744b1ccf93e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 78efcd28-7095-49f7-b660-9744b1ccf93e, GetRectangle, GetRectangle method [Tablet PC], GetRectangle method [Tablet PC],IInkRectangle interface, IInkRectangle interface [Tablet PC],GetRectangle method, IInkRectangle.GetRectangle, IInkRectangle::GetRectangle, msinkaut/IInkRectangle::GetRectangle, tablet.inkrectangle_getrectangle
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
 - IInkRectangle.GetRectangle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInkRectangle::GetRectangle


## -description



Gets the elements of the <a href="https://msdn.microsoft.com/78e6c29c-0f43-46a5-9d30-948de5f369c8">InkRectangle</a> object in a single call.




## -parameters




### -param Top [out]

The top of the rectangle.


### -param Left [out]

The left edge of the rectangle.


### -param Bottom [out]

The bottom of the rectangle.


### -param Right [out]

The right edge of the rectangle.


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
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/9b388cdb-66b1-4386-a1aa-578f0d56c190">Bottom Property</a>



<a href="https://msdn.microsoft.com/en-us/library/Mt846804(v=VS.85).aspx">IInkRectangle</a>



<a href="https://msdn.microsoft.com/78e6c29c-0f43-46a5-9d30-948de5f369c8">InkRectangle Class</a>



<a href="https://msdn.microsoft.com/88f0d919-43d0-408f-97f8-1410b2833269">Left Property</a>



<a href="https://msdn.microsoft.com/c31fd527-a6aa-4017-bc51-cedca42817f9">Right Property</a>



<a href="https://msdn.microsoft.com/f97145cf-9de9-427a-9701-36c6f4286910">Top Property</a>
 

 

