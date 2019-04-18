---
UID: NF:strmif.IDvdInfo2.GetDecoderCaps
title: IDvdInfo2::GetDecoderCaps (strmif.h)
author: windows-sdk-content
description: The GetDecoderCaps method retrieves the DVD decoder's maximum data rate for video, audio, and subpicture (in forward and reverse) as well as support for various types of audio (AC-3, MPEG-2, DTS, SDDS, LPCM).
old-location: dshow\idvdinfo2_getdecodercaps.htm
tech.root: DirectShow
ms.assetid: cfaf475c-336a-492f-b5a8-c49c21e5392d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetDecoderCaps, GetDecoderCaps method [DirectShow], GetDecoderCaps method [DirectShow],IDvdInfo2 interface, IDvdInfo2 interface [DirectShow],GetDecoderCaps method, IDvdInfo2.GetDecoderCaps, IDvdInfo2::GetDecoderCaps, IDvdInfo2GetDecoderCaps, dshow.idvdinfo2_getdecodercaps, strmif/IDvdInfo2::GetDecoderCaps
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
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
 - IDvdInfo2.GetDecoderCaps
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDvdInfo2::GetDecoderCaps


## -description



The <code>GetDecoderCaps</code> method retrieves the DVD decoder's maximum data rate for video, audio, and subpicture (in forward and reverse) as well as support for various types of audio (AC-3, MPEG-2, DTS, SDDS, LPCM).




## -parameters




### -param pCaps [out]

Pointer to a variable of type <a href="https://msdn.microsoft.com/7bfe5922-5d84-4ec8-87a0-e9bad102508b">DVD_DECODER_CAPS</a> that receives the information about the decoder.


## -returns



Returns one of the following <b>HRESULT</b> values.

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
<dt><b>VFW_E_WRONG_STATE</b></dt>
</dl>
</td>
<td width="60%">
The filter graph has not been initialized.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/6f41e0f1-e550-4ca6-9a80-ce4d498289e2">DVD Applications</a>



<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/da30d3dc-feec-4f54-b2db-a771ce404286">IDvdInfo2 Interface</a>
 

 

