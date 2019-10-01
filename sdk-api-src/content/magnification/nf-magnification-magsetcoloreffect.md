---
UID: NF:magnification.MagSetColorEffect
title: MagSetColorEffect function (magnification.h)
author: windows-sdk-content
description: Sets the color transformation matrix for a magnifier control.
old-location: magapi\magapi_MagSetColorEffect.htm
tech.root: magapi
ms.assetid: VS|magapi|~\magapi\reference\functions\magsetcoloreffect.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: MagSetColorEffect, MagSetColorEffect function [Magnification API], magapi.magapi_MagSetColorEffect, magapi_MagSetColorEffect, magnification/MagSetColorEffect
ms.topic: function
f1_keywords: 
 - "magnification/MagSetColorEffect"
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
 - MagSetColorEffect
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# MagSetColorEffect function


## -description


Sets the color transformation matrix for a magnifier control.


## -parameters




### -param hwnd [in]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">HWND</a></b>

The magnification window.


### -param pEffect [in]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/magnification/ns-magnification-magcoloreffect">PMAGCOLOREFFECT</a></b>

The color transformation matrix, or <b>NULL</b> to remove the current color effect, if any.


## -returns



Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">BOOL</a></b>

Returns <b>TRUE</b> if successful, or <b>FALSE</b> otherwise.




## -remarks



The magnifier control uses the color transformation matrix to apply a color effect to the entire magnifier window. If the function is called multiple times, the most recent color transform is used.

This function requires Windows Display Driver Model (WDDM)-capable video cards.


#### Examples

The following example sets a color transformation matrix that converts the colors displayed in the magnifier to grayscale.


```cpp
// Description:
//   Converts the colors displayed in the magnifier window to grayscale, or
//   returns the colors to normal.
// Parameters:
//   hwndMag - Handle of the magnifier control.
//   fInvert - TRUE to convert to grayscale, or FALSE for normal colors.
//
BOOL ConvertToGrayscale(HWND hwndMag, BOOL fConvert)
{
    // Convert the screen colors in the magnifier window.
    if (fConvert)
    {
        MAGCOLOREFFECT magEffectGrayscale = 
            {{ // MagEffectGrayscale
                {  0.3f,  0.3f,  0.3f,  0.0f,  0.0f },
                {  0.6f,  0.6f,  0.6f,  0.0f,  0.0f },
                {  0.1f,  0.1f,  0.1f,  0.0f,  0.0f },
                {  0.0f,  0.0f,  0.0f,  1.0f,  0.0f },
                {  0.0f,  0.0f,  0.0f,  0.0f,  1.0f } 
            }};

        return MagSetColorEffect(hwndMag, &magEffectGrayscale);
    }

    // Return the colors to normal.
    else
    {
        return MagSetColorEffect(hwndMag, NULL);
    }
}

```





## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/magnification/nf-magnification-maggetcoloreffect">MagGetColorEffect</a>
 

 

