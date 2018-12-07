---
UID: NF:d3d11_1.ID3D11VideoContext1.SubmitDecoderBuffers1
title: ID3D11VideoContext1::SubmitDecoderBuffers1
author: windows-sdk-content
description: Submits one or more buffers for decoding.
old-location: mf\id3d11videocontext1_submitdecoderbuffers1.htm
tech.root: medfound
ms.assetid: 9E5FC926-71D7-4102-8952-EC0585B4A4FC
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3D11VideoContext1 interface [Media Foundation],SubmitDecoderBuffers1 method, ID3D11VideoContext1.SubmitDecoderBuffers1, ID3D11VideoContext1::SubmitDecoderBuffers1, SubmitDecoderBuffers1, SubmitDecoderBuffers1 method [Media Foundation], SubmitDecoderBuffers1 method [Media Foundation],ID3D11VideoContext1 interface, d3d11_1/ID3D11VideoContext1::SubmitDecoderBuffers1, mf.id3d11videocontext1_submitdecoderbuffers1
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ID3D11VideoContext1.SubmitDecoderBuffers1
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11VideoContext1::SubmitDecoderBuffers1


## -description


Submits one or more buffers for decoding.


## -parameters




### -param pDecoder [in]

Type: <b>ID3D11VideoDecoder*</b>

A pointer to the <a href="https://msdn.microsoft.com/en-us/library/Hh447766(v=VS.85).aspx">ID3D11VideoDecoder</a> interface. To get this pointer, call the <a href="https://msdn.microsoft.com/en-us/library/Hh447786(v=VS.85).aspx">ID3D11VideoDevice::CreateVideoDecoder</a> method.


### -param NumBuffers [in]

Type: <b>UINT</b>

The number of buffers submitted for decoding.


### -param pBufferDesc [in]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/Dn894119(v=VS.85).aspx">D3D11_VIDEO_DECODER_BUFFER_DESC1</a>*</b>

A pointer to an array of <a href="https://msdn.microsoft.com/en-us/library/Dn894119(v=VS.85).aspx">D3D11_VIDEO_DECODER_BUFFER_DESC1</a> structures. The <i>NumBuffers</i> parameter specifies the number of elements in the array. Each element in the array describes a compressed buffer for decoding.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns S_OK. Otherwise, it returns an HRESULT error code.




## -remarks



This function does not honor any D3D11 predicate that may have been set.

<a href="https://msdn.microsoft.com/en-us/library/Ff476192(v=VS.85).aspx">D3D11_QUERY_DATA_PIPELINE_STATISTICS</a> will not include this function for any feature level.





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn894126(v=VS.85).aspx">ID3D11VideoContext1</a>
 

 

