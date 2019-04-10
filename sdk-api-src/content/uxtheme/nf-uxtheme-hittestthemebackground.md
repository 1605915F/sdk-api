---
UID: NF:uxtheme.HitTestThemeBackground
title: HitTestThemeBackground function (uxtheme.h)
author: windows-sdk-content
description: Retrieves a hit test code for a point in the background specified by a visual style.
old-location: controls\HitTestThemeBackground.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\userex\functions\hittestthemebackground.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: HitTestThemeBackground, HitTestThemeBackground function [Windows Controls], controls.HitTestThemeBackground, controls.inet_HitTestThemeBackground, inet_HitTestThemeBackground, inet_HitTestThemeBackground_cpp, uxtheme/HitTestThemeBackground
ms.topic: function
req.header: uxtheme.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: UxTheme.lib
req.dll: UxTheme.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - UxTheme.dll
api_name:
 - HitTestThemeBackground
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# HitTestThemeBackground function


## -description


Retrieves a hit test code for a point in the background specified by a visual style.


## -parameters




### -param hTheme [in]

Type: <b>HTHEME</b>

Handle to a window's specified theme data. Use <a href="https://msdn.microsoft.com/en-us/library/Bb759821(v=VS.85).aspx">OpenThemeData</a> to create an HTHEME.


### -param hdc [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HDC</a></b>

HDC to use when drawing. This parameter may be set to <b>NULL</b>.


### -param iPartId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the part. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param iStateId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the state of the part. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param dwOptions [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

<b>DWORD</b> that specifies the hit test options. See <a href="https://msdn.microsoft.com/en-us/library/Bb773203(v=VS.85).aspx">Hit Test Options</a> for a list of options.


### -param pRect [in]

Type: <b>LPCRECT</b>

Pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that contains, in logical coordinates, the rectangle that bounds the background.


### -param hrgn [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRGN</a></b>

Handle to a region that can be used to specify the bounds of a hit test area. This parameter may be set to <b>NULL</b>.


### -param ptTest [in]

Type: <b><a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a></b>


<a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a> structure that contains the coordinates of the point.


### -param pwHitTestCode [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">WORD</a>*</b>

<b>WORD</b> that receives the hit test code that indicates whether the point in <i>ptTest</i> is in the background area bounded by <i>pRect</i> or <i>hrgn</i>. See <a href="https://msdn.microsoft.com/en-us/library/Bb773206(v=VS.85).aspx">Hit Test Return Values</a> for a list of values returned.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The values in <i>ptTest</i> and <i>pRect</i> should be in the same coordinate system, such as client or screen. If the <i>hrgn</i> parameter is used, it must be specified in the same coordinates as <i>pRect</i> and <i>ptTest</i>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb773213(v=VS.85).aspx">Property Identifiers</a>
 

 

