---
UID: NF:magnification.MagGetImageScalingCallback
title: MagGetImageScalingCallback function (magnification.h)
author: windows-sdk-content
description: Retrieves the registered callback function that implements a custom transform for image scaling.
old-location: magapi\magapi_MagGetImageScalingCallback.htm
tech.root: magapi
ms.assetid: VS|magapi|~\magapi\reference\functions\maggetimagescalingcallback.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: MagGetImageScalingCallback, MagGetImageScalingCallback function [Magnification API], magapi.magapi_MagGetImageScalingCallback, magapi_MagGetImageScalingCallback, magnification/MagGetImageScalingCallback
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
 - MagGetImageScalingCallback
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# MagGetImageScalingCallback function


## -description



<div class="alert"><b>Note</b>  The <b>MagGetImageScalingCallback</b> function is deprecated in Windows 7 and later, and should not be used in new applications.  There is no alternate functionality.</div>
<div> </div>


Retrieves the registered callback function that implements a custom transform for image scaling. 


## -parameters




### -param hwnd [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

The magnification window.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms692392(v=VS.85).aspx">MagImageScalingCallback</a></b>

Returns the registered <a href="https://msdn.microsoft.com/en-us/library/ms692392(v=VS.85).aspx">MagImageScalingCallback</a> callback function, or <b>NULL</b> if no callback is registered.




## -remarks



This function returns <b>NULL</b> if Windows Display Driver Model (WDDM) is not supported.

This function works only when <a href="https://msdn.microsoft.com/en-us/library/Aa969540(v=VS.85).aspx">Desktop Window Manager</a> (DWM) is off.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms692392(v=VS.85).aspx">MagImageScalingCallback</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692395(v=VS.85).aspx">MagSetImageScalingCallback</a>
 

 

