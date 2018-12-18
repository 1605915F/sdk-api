---
UID: NF:uxtheme.GetThemeBackgroundExtent
title: GetThemeBackgroundExtent function
author: windows-sdk-content
description: Calculates the size and location of the background, defined by the visual style, given the content area.
old-location: controls\GetThemeBackgroundExtent.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\userex\functions\getthemebackgroundextent.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetThemeBackgroundExtent, GetThemeBackgroundExtent function [Windows Controls], controls.GetThemeBackgroundExtent, controls.inet_GetThemeBackgroundExtent, inet_GetThemeBackgroundExtent, inet_GetThemeBackgroundExtent_cpp, uxtheme/GetThemeBackgroundExtent
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
 - Ext-MS-Win-UXTheme-Themes-l1-1-0.dll
 - xamlpalwp.dll
 - ext-ms-win-uxtheme-themes-l1-1-1.dll
api_name:
 - GetThemeBackgroundExtent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetThemeBackgroundExtent function


## -description


Calculates the size and location of the background, defined by the visual style, given the content area.


## -parameters




### -param hTheme [in]

Type: <b>HTHEME</b>

Handle to a window's specified theme data. Use <a href="https://msdn.microsoft.com/en-us/library/Bb759821(v=VS.85).aspx">OpenThemeData</a> to create an HTHEME.


### -param hdc [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HDC</a></b>

HDC to use when drawing. This parameter may be set to <b>NULL</b>.


### -param iPartId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the part that contains the content. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param iStateId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the state of the part that contains the content. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param pContentRect [in]

Type: <b>LPCRECT</b>

Pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that contains the content background rectangle, in logical coordinates. This rectangle is returned from <a href="https://msdn.microsoft.com/en-us/library/Bb773375(v=VS.85).aspx">GetThemeBackgroundContentRect</a>.


### -param pExtentRect [out]

Type: <b>LPRECT</b>

Pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that receives the background rectangle, in logical coordinates. This rectangle is based on the <i>pContentRect</i>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



A theme can define a content area within each background image. This is the area where content such as text and icons can be placed without overwriting background borders.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb773375(v=VS.85).aspx">GetThemeBackgroundContentRect</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb773213(v=VS.85).aspx">Property Identifiers</a>



<b>Reference</b>
 

 

