---
UID: NF:iwstdec.IAMWstDecoder.GetRedrawAlways
title: IAMWstDecoder::GetRedrawAlways (iwstdec.h)
author: windows-sdk-content
description: Downstream filters use the GetRedrawAlways method to retrieve a value that indicates whether the whole output bitmap is redrawn for each sample.
old-location: dshow\iamwstdecoder_getredrawalways.htm
tech.root: DirectShow
ms.assetid: d4035bd0-9a86-4deb-b4eb-4aa5b4b4ff35
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRedrawAlways, GetRedrawAlways method [DirectShow], GetRedrawAlways method [DirectShow],IAMWstDecoder interface, IAMWstDecoder interface [DirectShow],GetRedrawAlways method, IAMWstDecoder.GetRedrawAlways, IAMWstDecoder::GetRedrawAlways, IAMWstDecoderGetRedrawAlways, dshow.iamwstdecoder_getredrawalways, iwstdec/IAMWstDecoder::GetRedrawAlways
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
 - IAMWstDecoder.GetRedrawAlways
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMWstDecoder::GetRedrawAlways


## -description



Downstream filters use the <code>GetRedrawAlways</code> method to retrieve a value that indicates whether the whole output bitmap is redrawn for each sample.




## -parameters




### -param lpbOption [out]

Pointer to a <b>BOOL</b> to receive the redraw-always value.

<table>
<tr>
<th>Value
                </th>
<th>Description
                </th>
</tr>
<tr>
<td><b>TRUE</b></td>
<td>Redraw the whole output bitmap for each sample.</td>
</tr>
<tr>
<td><b>FALSE</b></td>
<td>Do not redraw the whole output bitmap for each sample.</td>
</tr>
</table>
 


## -returns



When the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd376041(v=VS.85).aspx">IAMWstDecoder Interface</a>
 

 

