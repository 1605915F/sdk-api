---
UID: NF:tapi3ds.ITAMMediaFormat.get_MediaFormat
title: ITAMMediaFormat::get_MediaFormat
author: windows-sdk-content
description: The get_MediaFormat method gets the media format.
old-location: tapi3\itammediaformat_get_mediaformat.htm
tech.root: Tapi
ms.assetid: 384cd41e-b59a-4ac4-9687-cf0f0738dfe0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITAMMediaFormat interface [TAPI 2.2],get_MediaFormat method, ITAMMediaFormat.get_MediaFormat, ITAMMediaFormat::get_MediaFormat, _tapi3_itammediaformat_get_mediaformat, get_MediaFormat, get_MediaFormat method [TAPI 2.2], get_MediaFormat method [TAPI 2.2],ITAMMediaFormat interface, tapi3.itammediaformat_get_mediaformat, tapi3ds/ITAMMediaFormat::get_MediaFormat
ms.topic: method
req.header: tapi3ds.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITAMMediaFormat.get_MediaFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITAMMediaFormat::get_MediaFormat


## -description


The 
<b>get_MediaFormat</b> method gets the media format.


## -parameters




### -param ppmt [out]

Pointer to an array of 
<b>AM_MEDIA_TYPE</b> structures. For more information on <b>AM_MEDIA_TYPE</b>, see the DirectX documentation. 


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
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/82728afe-5743-4b45-86e6-32df021a2a5f">ITAMMediaFormat</a>



<a href="https://msdn.microsoft.com/0d96f229-76c0-46a3-bc4b-6f558b9956c6">Terminal Object</a>



<a href="https://msdn.microsoft.com/692df069-3016-46a2-9f33-4c709e85be1b">put_MediaFormat</a>
 

 

