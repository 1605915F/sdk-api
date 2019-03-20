---
UID: NF:segment.IMSVidEncoder.get_VideoEncoderInterface
title: IMSVidEncoder::get_VideoEncoderInterface (segment.h)
author: windows-sdk-content
description: The get_VideoEncoderInterface method retrieves a pointer to the video encoder interface.
old-location: mstv\imsvidencoder_get_videoencoderinterface.htm
tech.root: mstv
ms.assetid: c6ee3169-ba24-495f-b446-161c899aab16
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidEncoder interface [Microsoft TV Technologies],get_VideoEncoderInterface method, IMSVidEncoder.get_VideoEncoderInterface, IMSVidEncoder::get_VideoEncoderInterface, IMSVidEncoderget_VideoEncoderInterface, get_VideoEncoderInterface, get_VideoEncoderInterface method [Microsoft TV Technologies], get_VideoEncoderInterface method [Microsoft TV Technologies],IMSVidEncoder interface, mstv.imsvidencoder_get_videoencoderinterface, segment/IMSVidEncoder::get_VideoEncoderInterface
ms.topic: method
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Segment.idl
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
 - segment.h
api_name:
 - IMSVidEncoder.get_VideoEncoderInterface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidEncoder::get_VideoEncoderInterface


## -description


The <b>get_VideoEncoderInterface</b> method retrieves a pointer to the video encoder interface.


## -parameters




### -param ppEncInt [out]

Pointer to a variable that receives an <b>IUnknown</b> interface pointer. The caller can query this interface for the <a href="https://msdn.microsoft.com/en-us/library/Dd693975(v=VS.85).aspx">IEncoderAPI</a> interface.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -remarks



If the method succeeds, the caller must release the <b>IUnknown</b> interface.




## -see-also




<a href="https://msdn.microsoft.com/37d03dff-ae40-4e7f-a66f-facd0c1f6eee">IMSVidEncoder Interface</a>
 

 

