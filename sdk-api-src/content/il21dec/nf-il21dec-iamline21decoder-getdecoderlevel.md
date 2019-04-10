---
UID: NF:il21dec.IAMLine21Decoder.GetDecoderLevel
title: IAMLine21Decoder::GetDecoderLevel (il21dec.h)
author: windows-sdk-content
description: The GetDecoderLevel method retrieves the closed-captioned decoder level.
old-location: dshow\iamline21decoder_getdecoderlevel.htm
tech.root: DirectShow
ms.assetid: 6f0fc2c3-cc98-4646-ada0-57d74c6b5dd9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetDecoderLevel, GetDecoderLevel method [DirectShow], GetDecoderLevel method [DirectShow],IAMLine21Decoder interface, IAMLine21Decoder interface [DirectShow],GetDecoderLevel method, IAMLine21Decoder.GetDecoderLevel, IAMLine21Decoder::GetDecoderLevel, IAMLine21DecoderGetDecoderLevel, dshow.iamline21decoder_getdecoderlevel, il21dec/IAMLine21Decoder::GetDecoderLevel
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
 - IAMLine21Decoder.GetDecoderLevel
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMLine21Decoder::GetDecoderLevel


## -description



The <code>GetDecoderLevel</code> method retrieves the closed-captioned decoder level.




## -parameters




### -param lpLevel

Pointer to a variable that receives a member of the <a href="https://msdn.microsoft.com/en-us/library/Dd373473(v=VS.85).aspx">AM_LINE21_CCLEVEL</a> enumeration. The returned value is always <b>AM_L21_CCLEVEL_TC2</b> (TeleCaption II).


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
</table>
 




## -remarks



TeleCaption I and TeleCaption II are standards for closed caption decoders. The <a href="https://msdn.microsoft.com/48fa5484-1f8c-4133-b2e1-888cb1834402">Line 21 Decoder</a> filter supports TeleCaption II, which is backward compatible with TeleCaption I.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd389385(v=VS.85).aspx">IAMLine21Decoder Interface</a>
 

 

