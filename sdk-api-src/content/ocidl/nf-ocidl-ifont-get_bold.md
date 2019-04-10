---
UID: NF:ocidl.IFont.get_Bold
title: IFont::get_Bold (ocidl.h)
author: windows-sdk-content
description: Gets the font's current Bold property.
old-location: com\ifont_get_bold.htm
tech.root: com
ms.assetid: bc0a8353-852b-4314-83b1-a07321159945
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IFont interface [COM],get_Bold method, IFont.get_Bold, IFont::get_Bold, _ctrl_ifont_get_bold, com.ifont_get_bold, get_Bold, get_Bold method [COM], get_Bold method [COM],IFont interface, ocidl/IFont::get_Bold
ms.topic: method
req.header: ocidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OCIdl.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - OCIdl.h
api_name:
 - IFont.get_Bold
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFont::get_Bold


## -description


Gets the font's current Bold property.


## -parameters




### -param pBold [out]

A pointer to a caller-allocated 
     variable that receives the current Bold property for the font.


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
<dt><b>S_OK </b></dt>
</dl>
</td>
<td width="60%">
The state was retrieved successfully. If the state is indeterminate, a font object should set *<i>pBold</i> to <b>FALSE</b> and return <b>S_OK</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The address in pBold is not valid. For example, it may be <b>NULL</b>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/3a04d2b7-b2eb-4c6c-8863-1e88321fa382">IFont</a>



<a href="https://msdn.microsoft.com/c25738fe-daf4-4eac-b4b0-354950e29f27">IFont::put_Bold</a>
 

 

