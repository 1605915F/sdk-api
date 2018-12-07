---
UID: NF:strmif.IAMVideoCompression.put_PFramesPerKeyFrame
title: IAMVideoCompression::put_PFramesPerKeyFrame
author: windows-sdk-content
description: The put_PFramesPerKeyFrame method sets the rate of predicted (P) frames per key frame.
old-location: dshow\iamvideocompression_put_pframesperkeyframe.htm
tech.root: DirectShow
ms.assetid: bf1dfc28-a6c7-4c0d-96ea-8cf417b13a10
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAMVideoCompression interface [DirectShow],put_PFramesPerKeyFrame method, IAMVideoCompression.put_PFramesPerKeyFrame, IAMVideoCompression::put_PFramesPerKeyFrame, IAMVideoCompressionput_PFramesPerKeyFrame, dshow.iamvideocompression_put_pframesperkeyframe, put_PFramesPerKeyFrame, put_PFramesPerKeyFrame method [DirectShow], put_PFramesPerKeyFrame method [DirectShow],IAMVideoCompression interface, strmif/IAMVideoCompression::put_PFramesPerKeyFrame
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: strmif.h
req.include-header: Dshow.h
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
 - IAMVideoCompression.put_PFramesPerKeyFrame
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMVideoCompression::put_PFramesPerKeyFrame


## -description



The <code>put_PFramesPerKeyFrame</code> method sets the rate of predicted (P) frames per key frame.




## -parameters




### -param PFramesPerKeyFrame [in]

Specifies the number of P frames per key frame. If the value is negative, the filter will use the default rate.


## -returns



Returns an <b>HRESULT</b> value.




## -remarks



To determine if the filter supports this method, call the <a href="https://msdn.microsoft.com/d8ba2ba2-510a-4fb8-844e-48059ec4ef0d">IAMVideoCompression::GetInfo</a> method and check for the <b>CompressionCaps_CanBFrame</b> flag in the <i>pCapabilities</i> parameter. The <b>GetInfo</b> method also returns the default P-frame rate.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/6b7d8a98-35b8-442f-bf51-9e66fd03e2c9">IAMVideoCompression Interface</a>



<a href="https://msdn.microsoft.com/621292dd-42d9-4458-8971-929db39ed8b9">IAMVideoCompression::get_PFramesPerKeyFrame</a>
 

 

