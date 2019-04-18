---
UID: NF:il21dec.IAMLine21Decoder.GetOutputFormat
title: IAMLine21Decoder::GetOutputFormat (il21dec.h)
author: windows-sdk-content
description: The GetOutputFormat method retrieves the Line 21 Decoder filter's output format.
old-location: dshow\iamline21decoder_getoutputformat.htm
tech.root: DirectShow
ms.assetid: 3d1ded3c-fdeb-4e02-92ee-d0986711c335
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetOutputFormat, GetOutputFormat method [DirectShow], GetOutputFormat method [DirectShow],IAMLine21Decoder interface, IAMLine21Decoder interface [DirectShow],GetOutputFormat method, IAMLine21Decoder.GetOutputFormat, IAMLine21Decoder::GetOutputFormat, IAMLine21DecoderGetOutputFormat, dshow.iamline21decoder_getoutputformat, il21dec/IAMLine21Decoder::GetOutputFormat
ms.topic: method
req.header: il21dec.h
req.include-header: 
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IAMLine21Decoder.GetOutputFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAMLine21Decoder::GetOutputFormat


## -description



The <code>GetOutputFormat</code> method retrieves the <a href="https://msdn.microsoft.com/48fa5484-1f8c-4133-b2e1-888cb1834402">Line 21 Decoder</a> filter's output format.




## -parameters




### -param lpbmih

Pointer to a caller-allocated <a href="https://msdn.microsoft.com/153c08a8-d32c-4e9d-9da9-b915eb172327">BITMAPINFOHEADER</a> structure.


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The output format has not been set.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd389385(v=VS.85).aspx">IAMLine21Decoder Interface</a>
 

 

