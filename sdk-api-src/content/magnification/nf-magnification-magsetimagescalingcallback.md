---
UID: NF:magnification.MagSetImageScalingCallback
title: MagSetImageScalingCallback function
author: windows-sdk-content
description: Sets the callback function for external image filtering and scaling.
old-location: magapi\magapi_MagSetImageScalingCallback.htm
tech.root: magapi
ms.assetid: VS|magapi|~\magapi\reference\functions\magsetimagescalingcallback.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MagSetImageScalingCallback, MagSetImageScalingCallback function [Magnification API], magapi.magapi_MagSetImageScalingCallback, magapi_MagSetImageScalingCallback, magnification/MagSetImageScalingCallback
ms.topic: function
req.header: magnification.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Magnification.lib
req.dll: Magnification.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Magnification.dll
api_name:
 - MagSetImageScalingCallback
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MagSetImageScalingCallback function


## -description



<div class="alert"><b>Note</b>  The <b>MagSetImageScalingCallback</b> function is deprecated in Windows 7 and later, and should not be used in new applications.  There is no alternate functionality.</div>
<div> </div>


Sets the callback function for external image filtering and scaling.


## -parameters




### -param hwnd [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

The handle of the magnification window.


### -param callback [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms692392(v=VS.85).aspx">MagImageScalingCallback</a></b>

The callback function, or <b>NULL</b> to remove a callback that was previously set.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

Returns <b>TRUE</b> if successful, or <b>FALSE</b> otherwise.




## -remarks



This function requires Windows Display Driver Model (WDDM)-capable video cards.

This function works only when <a href="https://msdn.microsoft.com/en-us/library/Aa969540(v=VS.85).aspx">Desktop Window Manager</a> (DWM) is off.

This callback mechanism enables custom image filtering and scaling mechanisms. Filtering might include bilinear, trilinear, bicubic, and flat. The mechanism also enables edge detection and enhancement.

The only transform that can be performed within the callback is scaling. Rotations and skews that may compose the arbitrary transform passed to the <a href="https://msdn.microsoft.com/en-us/library/ms692398(v=VS.85).aspx">MagSetWindowTransform</a> function are performed after the callback function returns.

The specified function is called by the magnification engine for all rasterized Windows Graphics Device Interface (GDI) bitmaps before they are composited.

	
After the callback function returns, the bitmap in video memory can have one of the following size states:


<ul>
<li>Unscaled. The returned bitmap is the same size as the bitmap passed by the caller. The magnification engine does the scaling 
by the transform specified in the <a href="https://msdn.microsoft.com/en-us/library/ms692398(v=VS.85).aspx">MagSetWindowTransform</a> function.
</li>
<li>Scaled. The returned bitmap is scaled by the transform specified in <a href="https://msdn.microsoft.com/en-us/library/ms692398(v=VS.85).aspx">MagSetWindowTransform</a>.
</li>
</ul>
If no callback is registered, the magnification engine scales bitmaps by the transform specified in <a href="https://msdn.microsoft.com/en-us/library/ms692398(v=VS.85).aspx">MagSetWindowTransform</a>.


Windows Presentation Foundation (WPF) bitmaps can be scaled automatically using flat, bilinear, bicubic filtering and 
consequently do not use this callback mechanism.





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms692388(v=VS.85).aspx">MagGetImageScalingCallback</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692395(v=VS.85).aspx">MagSetImageScalingCallback</a>
 

 

