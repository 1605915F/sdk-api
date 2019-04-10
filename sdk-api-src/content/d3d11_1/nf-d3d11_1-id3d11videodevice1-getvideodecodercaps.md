---
UID: NF:d3d11_1.ID3D11VideoDevice1.GetVideoDecoderCaps
title: ID3D11VideoDevice1::GetVideoDecoderCaps (d3d11_1.h)
author: windows-sdk-content
description: Retrieves capabilities and limitations of the video decoder.
old-location: mf\id3d11videodevice1_getvideodecodercaps.htm
tech.root: medfound
ms.assetid: 9F978BE5-568E-440C-B9B2-0972893FD970
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetVideoDecoderCaps, GetVideoDecoderCaps method [Media Foundation], GetVideoDecoderCaps method [Media Foundation],ID3D11VideoDevice1 interface, ID3D11VideoDevice1 interface [Media Foundation],GetVideoDecoderCaps method, ID3D11VideoDevice1.GetVideoDecoderCaps, ID3D11VideoDevice1::GetVideoDecoderCaps, d3d11_1/ID3D11VideoDevice1::GetVideoDecoderCaps, mf.id3d11videodevice1_getvideodecodercaps
ms.topic: method
req.header: d3d11_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
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
 - d3d11_1.h
api_name:
 - ID3D11VideoDevice1.GetVideoDecoderCaps
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11VideoDevice1::GetVideoDecoderCaps


## -description


Retrieves capabilities and limitations of the video decoder.


## -parameters




### -param pDecoderProfile [in]

Type: <b>const GUID*</b>

The decode profile for which the capabilities are queried.


### -param SampleWidth [in]

Type: <b>UINT</b>

The video width for which the capabilities are queried.


### -param SampleHeight [in]

Type: <b>UINT</b>

The video height for which the capabilities are queried.


### -param pFrameRate [in]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/Bb173069(v=VS.85).aspx">DXGI_RATIONAL</a>*</b>

The frame rate of the video content. This information is used by the driver to determine whether the video can be decoded in real-time.


### -param BitRate [in]

Type: <b>UINT</b>

The bit rate of the video stream. A value of zero indicates that the bit rate can be ignored.


### -param pCryptoType [in]

Type: <b>const GUID*</b>

The type of cryptography used to encrypt the video stream. A value of NULL indicates that the video stream is not encrypted.


### -param pDecoderCaps [out]

Type: <b>UINT*</b>

A pointer to a bitwise OR combination of <a href="https://msdn.microsoft.com/8E3C86A4-5F73-4E6F-8F93-5564EA0BC113">D3D11_VIDEO_DECODER_CAPS</a> values specifying the decoder capabilities.




## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the following error codes.

<table>
<tr>
<td>S_OK</td>
<td>The operation completed successfully.</td>
</tr>
<tr>
<td>E_INVALIDARG</td>
<td>An invalid parameter was passed or this function was called using an invalid calling pattern.</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/10E68945-6103-491D-8846-3B7C880FEAFD">ID3D11VideoDevice1</a>
 

 

