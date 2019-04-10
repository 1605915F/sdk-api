---
UID: NF:wincodec.IWICDdsFrameDecode.CopyBlocks
title: IWICDdsFrameDecode::CopyBlocks (wincodec.h)
author: windows-sdk-content
description: Requests pixel data as it is natively stored within the DDS file.
old-location: wic\iwicddsframedecode_copyblocks.htm
tech.root: wic
ms.assetid: D090AA8E-46F2-40C9-A156-12038053E040
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CopyBlocks, CopyBlocks method [Windows Imaging Component], CopyBlocks method [Windows Imaging Component],IWICDdsFrameDecode interface, IWICDdsFrameDecode interface [Windows Imaging Component],CopyBlocks method, IWICDdsFrameDecode.CopyBlocks, IWICDdsFrameDecode::CopyBlocks, wic.iwicddsframedecode_copyblocks, wincodec/IWICDdsFrameDecode::CopyBlocks
ms.topic: method
req.header: wincodec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wincodec.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Windowscodecs.lib
req.dll: Windowscodecs.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Windowscodecs.dll
api_name:
 - IWICDdsFrameDecode.CopyBlocks
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWICDdsFrameDecode::CopyBlocks


## -description


Requests pixel data as it is natively stored within the DDS file.


## -parameters




### -param prcBoundsInBlocks [in]

Type: <b>const <a href="https://msdn.microsoft.com/e07c26bf-b645-4382-bb93-8472ba397026">WICRect</a>*</b>

The rectangle to copy from the source. A NULL value specifies the entire texture.

If the texture uses a block-compressed <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>, all values of the rectangle are expressed in number of blocks, not pixels.


### -param cbStride [in]

Type: <b>UINT</b>

The stride, in bytes, of the destination buffer. This represents the number of bytes from the buffer pointer to the next row of data. If the texture uses a block-compressed <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>, a "row of data" is defined as a row of blocks which contains multiple pixel scanlines.


### -param cbBufferSize [in]

Type: <b>UINT</b>

The size, in bytes, of the destination buffer.


### -param pbBuffer [out]

Type: <b>BYTE*</b>

A pointer to the destination buffer.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



If the texture does not use a block-compressed <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>, this method behaves similarly to <a href="https://msdn.microsoft.com/d4908a75-e7de-4b8f-bdc8-d86cf6b49f8c">IWICBitmapSource::CopyPixels</a>. However, it does not perform any pixel format conversion, and instead produces the raw data from the DDS file.

If the texture uses a block-compressed <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>, this method copies the block data directly into the provided buffer. In this case, the <i>prcBoundsInBlocks</i> parameter is defined in blocks, not pixels. To determine if this is the case, call <a href="https://msdn.microsoft.com/0D5B9E45-E1EA-4D16-B793-63FEAB2BAF65">GetFormatInfo</a> and read the <b>DxgiFormat</b> member of the returned <a href="https://msdn.microsoft.com/C5F1DA49-EC11-4068-9DC6-D721894371F9">WICDdsFormatInfo</a> structure.





## -see-also




<a href="https://msdn.microsoft.com/d4908a75-e7de-4b8f-bdc8-d86cf6b49f8c">IWICBitmapSource::CopyPixels</a>



<a href="https://msdn.microsoft.com/52E76A8D-E7E2-46F5-BBCC-B7C74F1B1122">IWICDdsFrameDecode</a>
 

 

