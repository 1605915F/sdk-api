---
UID: NF:segment.IMSVidRect.get_Top
title: IMSVidRect::get_Top
author: windows-sdk-content
description: The get_Top method retrieves the top y-coordinate of the rectangle. This coordinate is relative to the rectangle's associated window.
old-location: mstv\imsvidrect_get_top.htm
tech.root: mstv
ms.assetid: 3596141c-e359-4ea5-8d6a-9ec374c1f854
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidRect interface [Microsoft TV Technologies],get_Top method, IMSVidRect.get_Top, IMSVidRect::get_Top, IMSVidRectget_Top, get_Top, get_Top method [Microsoft TV Technologies], get_Top method [Microsoft TV Technologies],IMSVidRect interface, mstv.imsvidrect_get_top, segment/IMSVidRect::get_Top
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
 - IMSVidRect.get_Top
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidRect::get_Top


## -description


The <b>get_Top</b> method retrieves the top y-coordinate of the rectangle. This coordinate is relative to the rectangle's associated window.


## -parameters




### -param TopVal [out]

Pointer to a variable that receives the top y-coordinate, in pixels.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an error code.




## -see-also




<a href="https://msdn.microsoft.com/0b3cf31b-e0cc-4208-a128-b77460fc0f1b">IMSVidRect Interface</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd694605(v=VS.85).aspx">IMSVidRect::get_HWnd</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd694613(v=VS.85).aspx">IMSVidRect::put_Top</a>
 

 

