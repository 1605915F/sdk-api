---
UID: NF:iwstdec.IAMWstDecoder.SetOutputFormat
title: IAMWstDecoder::SetOutputFormat (iwstdec.h)
author: windows-sdk-content
description: Downstream filters use the SetOutputFormat method to define an output video format.
old-location: dshow\iamwstdecoder_setoutputformat.htm
tech.root: DirectShow
ms.assetid: 92d19d2b-dce5-4dd6-ac96-a39fa48fa1aa
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAMWstDecoder interface [DirectShow],SetOutputFormat method, IAMWstDecoder.SetOutputFormat, IAMWstDecoder::SetOutputFormat, IAMWstDecoderSetOutputFormat, SetOutputFormat, SetOutputFormat method [DirectShow], SetOutputFormat method [DirectShow],IAMWstDecoder interface, dshow.iamwstdecoder_setoutputformat, iwstdec/IAMWstDecoder::SetOutputFormat
ms.topic: method
req.header: iwstdec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - IAMWstDecoder.SetOutputFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMWstDecoder::SetOutputFormat


## -description



Downstream filters use the <code>SetOutputFormat</code> method to define an output video format.




## -parameters




### -param lpbmi [in]

A pointer to a  <b>BITMAPINFO</b> structure that describes the output video format, such as size, bit depth, and other properties.


## -returns



When the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
So far, downstream filters have defined no output format.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Downstream filters have already defined an output format.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376041(v=VS.85).aspx">IAMWstDecoder Interface</a>
 

 

