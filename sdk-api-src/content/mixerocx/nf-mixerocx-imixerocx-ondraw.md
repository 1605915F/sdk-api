---
UID: NF:mixerocx.IMixerOCX.OnDraw
title: IMixerOCX::OnDraw
author: windows-sdk-content
description: The OnDraw method instructs the Overlay Mixer to draw the video rectangle.
old-location: dshow\imixerocx_ondraw.htm
tech.root: DirectShow
ms.assetid: 69b8752b-9f97-422e-8a9a-f49c7a472cb6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMixerOCX interface [DirectShow],OnDraw method, IMixerOCX.OnDraw, IMixerOCX::OnDraw, IMixerOCXOnDraw, OnDraw, OnDraw method [DirectShow], OnDraw method [DirectShow],IMixerOCX interface, dshow.imixerocx_ondraw, mixerocx/IMixerOCX::OnDraw
ms.topic: method
req.header: mixerocx.h
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
 - IMixerOCX.OnDraw
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMixerOCX::OnDraw


## -description



The <code>OnDraw</code> method instructs the Overlay Mixer to draw the video rectangle.




## -parameters




### -param hdcDraw [in]

Specifies the device context associated with the parent window.


### -param prcDraw [in]

Specifies the rectangle coordinates of the video rectangle.


## -returns



If the method succeeds, it returns S_OK.




## -remarks



The HDC provided here should not be cached.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd407084(v=VS.85).aspx">IMixerOCX Interface</a>



<a href="https://msdn.microsoft.com/e80938b7-31f0-467b-a3fa-c4511d14758d">Overlay Mixer</a>
 

 

