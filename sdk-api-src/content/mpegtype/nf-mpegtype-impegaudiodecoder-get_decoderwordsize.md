---
UID: NF:mpegtype.IMpegAudioDecoder.get_DecoderWordSize
title: IMpegAudioDecoder::get_DecoderWordSize
author: windows-sdk-content
description: Returns the word size used to decode, either eight or 16 bit.
old-location: dshow\impegaudiodecoder_get_decoderwordsize.htm
tech.root: DirectShow
ms.assetid: 92528359-cdbf-4490-badd-1ad20643ec1a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMpegAudioDecoder interface [DirectShow],get_DecoderWordSize method, IMpegAudioDecoder.get_DecoderWordSize, IMpegAudioDecoder::get_DecoderWordSize, IMpegAudioDecodergetDecoderWordSize, dshow.impegaudiodecoder_get_decoderwordsize, get_DecoderWordSize, get_DecoderWordSize method [DirectShow], get_DecoderWordSize method [DirectShow],IMpegAudioDecoder interface, mpegtype/IMpegAudioDecoder::get_DecoderWordSize
ms.topic: method
req.header: mpegtype.h
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
 - IMpegAudioDecoder.get_DecoderWordSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMpegAudioDecoder::get_DecoderWordSize


## -description



Returns the word size used to decode, either eight or 16 bit.




## -parameters




### -param pWordSize [out]

Indicates the word size; the value is either 8 or 16.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

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
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd376656(v=VS.85).aspx">IMpegAudioDecoder</a>
 

 

