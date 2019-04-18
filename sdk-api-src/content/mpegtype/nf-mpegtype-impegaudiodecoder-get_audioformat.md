---
UID: NF:mpegtype.IMpegAudioDecoder.get_AudioFormat
title: IMpegAudioDecoder::get_AudioFormat (mpegtype.h)
author: windows-sdk-content
description: Returns the audio format of the connected input pin.
old-location: dshow\impegaudiodecoder_get_audioformat.htm
tech.root: DirectShow
ms.assetid: f7634504-d3f5-46a9-be25-08293190c27b
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IMpegAudioDecoder interface [DirectShow],get_AudioFormat method, IMpegAudioDecoder.get_AudioFormat, IMpegAudioDecoder::get_AudioFormat, IMpegAudioDecodergetAudioFormat, dshow.impegaudiodecoder_get_audioformat, get_AudioFormat, get_AudioFormat method [DirectShow], get_AudioFormat method [DirectShow],IMpegAudioDecoder interface, mpegtype/IMpegAudioDecoder::get_AudioFormat
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
 - IMpegAudioDecoder.get_AudioFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMpegAudioDecoder::get_AudioFormat


## -description



Returns the audio format of the connected input pin.




## -parameters




### -param lpFmt [out]

Pointer to an <a href="https://msdn.microsoft.com/c9357f72-f101-434a-b7ae-183e78239e9c">MPEG1WAVEFORMAT</a> structure. The method copies the format data into the structure.


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
 

 

