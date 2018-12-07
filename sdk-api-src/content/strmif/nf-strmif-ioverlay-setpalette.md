---
UID: NF:strmif.IOverlay.SetPalette
title: IOverlay::SetPalette
author: windows-sdk-content
description: The SetPalette method sets the palette.
old-location: dshow\ioverlay_setpalette.htm
tech.root: DirectShow
ms.assetid: 572f77ab-08a8-453a-993b-724da967bcde
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOverlay interface [DirectShow],SetPalette method, IOverlay.SetPalette, IOverlay::SetPalette, IOverlaySetPalette, SetPalette, SetPalette method [DirectShow], SetPalette method [DirectShow],IOverlay interface, dshow.ioverlay_setpalette, strmif/IOverlay::SetPalette
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
 - IOverlay.SetPalette
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOverlay::SetPalette


## -description



The <code>SetPalette</code> method sets the palette.




## -parameters




### -param dwColors [in]

Number of colors present.


### -param pPalette [in]

Pointer to colors to use for the palette.


## -returns



Returns S_OK if successful. If the method fails, it returns an <b>HRESULT</b> error code.




## -remarks



This method sets a logical palette for the window. The window is not guaranteed to always have the colors requested in the actual system device palette. The Microsoft® Windows® operating system only guarantees those colors when the window is the foreground active window. The current device palette can be obtained by calling <a href="https://msdn.microsoft.com/993c80fb-fa67-4dd6-815b-8e15d2f7f495">IOverlay::GetPalette</a>.

If the device does not have a palette, it returns VFW_E_NO_DISPLAY_PALETTE.

The <a href="https://msdn.microsoft.com/e80938b7-31f0-467b-a3fa-c4511d14758d">Overlay Mixer</a> filter returns E_NOTIMPL.




## -see-also




<a href="https://msdn.microsoft.com/369c2bd1-9c11-4524-b999-6a3b73c45261">Error and Success Codes</a>



<a href="https://msdn.microsoft.com/2d49888a-7046-4779-9634-d181fa582584">IOverlay Interface</a>
 

 

