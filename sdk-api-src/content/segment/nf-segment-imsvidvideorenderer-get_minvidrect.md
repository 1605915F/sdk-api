---
UID: NF:segment.IMSVidVideoRenderer.get_MinVidRect
title: IMSVidVideoRenderer::get_MinVidRect (segment.h)
author: windows-sdk-content
description: The get_MinVidRect method retrieves the minimum ideal size of the video rectangle.
old-location: mstv\imsvidvideorenderer_get_minvidrect.htm
tech.root: mstv
ms.assetid: 2e65f2b2-d479-429a-b5c7-8c5cbb6c833d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IMSVidVideoRenderer interface [Microsoft TV Technologies],get_MinVidRect method, IMSVidVideoRenderer.get_MinVidRect, IMSVidVideoRenderer::get_MinVidRect, IMSVidVideoRendererget_MinVidRect, get_MinVidRect, get_MinVidRect method [Microsoft TV Technologies], get_MinVidRect method [Microsoft TV Technologies],IMSVidVideoRenderer interface, mstv.imsvidvideorenderer_get_minvidrect, segment/IMSVidVideoRenderer::get_MinVidRect
ms.topic: method
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
 - IMSVidVideoRenderer.get_MinVidRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidVideoRenderer::get_MinVidRect


## -description


The <b>get_MinVidRect</b> method retrieves the minimum ideal size of the video rectangle.


## -parameters




### -param ppVidRect [out]

Receives an <a href="https://msdn.microsoft.com/0b3cf31b-e0cc-4208-a128-b77460fc0f1b">IMSVidRect</a> interface pointer.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -remarks



The minimum ideal image size is the minimum video size that can be displayed without significantly degrading performance or image quality.

The returned <a href="https://msdn.microsoft.com/0b3cf31b-e0cc-4208-a128-b77460fc0f1b">IMSVidRect</a> interface has an outstanding reference count. The caller must release the interface.




## -see-also




<a href="https://msdn.microsoft.com/27eb53f8-ece8-43eb-8f94-b3d2d91548ad">IMSVidVideoRenderer Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd694737(v=VS.85).aspx">IMSVidVideoRenderer::get_MaxVidRect</a>
 

 

