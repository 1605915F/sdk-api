---
UID: NF:wincodec.IWICJpegFrameDecode.GetFrameHeader
title: IWICJpegFrameDecode::GetFrameHeader
author: windows-sdk-content
description: Retrieves header data from the entire frame.
old-location: wic\iwicjpegframedecode_getframeheader.htm
tech.root: wic
ms.assetid: CE29251F-C2E2-422B-B6BD-034D6B479009
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetFrameHeader, GetFrameHeader method [Windows Imaging Component], GetFrameHeader method [Windows Imaging Component],IWICJpegFrameDecode interface, IWICJpegFrameDecode interface [Windows Imaging Component],GetFrameHeader method, IWICJpegFrameDecode.GetFrameHeader, IWICJpegFrameDecode::GetFrameHeader, wic.iwicjpegframedecode_getframeheader, wincodec/IWICJpegFrameDecode::GetFrameHeader
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wincodec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - IWICJpegFrameDecode.GetFrameHeader
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWICJpegFrameDecode::GetFrameHeader


## -description


Retrieves  header data from the entire frame.  The result includes parameters from the Start Of Frame (SOF) marker for the scan as well as parameters derived from other metadata such as the color model of the compressed data.


## -parameters




### -param pFrameHeader [out]

Type: <b><a href="https://msdn.microsoft.com/BB207D78-9E27-49A4-91E4-601CED109389">WICJpegFrameHeader</a>*</b>

A pointer that receives the frame header data.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns S_OK on successful completion.




## -see-also




<a href="https://msdn.microsoft.com/E6310320-53A8-40F1-8964-D21D8054E1B8">IWICJpegFrameDecode</a>



<a href="https://msdn.microsoft.com/BB207D78-9E27-49A4-91E4-601CED109389">WICJpegFrameHeader</a>
 

 

