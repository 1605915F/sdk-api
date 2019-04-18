---
UID: NF:uxtheme.GetThemePartSize
title: GetThemePartSize function (uxtheme.h)
author: windows-sdk-content
description: Calculates the original size of the part defined by a visual style.
old-location: controls\GetThemePartSize.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\userex\functions\getthemepartsize.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetThemePartSize, GetThemePartSize function [Windows Controls], controls.GetThemePartSize, controls.inet_GetThemePartSize, inet_GetThemePartSize, inet_GetThemePartSize_cpp, uxtheme/GetThemePartSize
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
 - GetThemePartSize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetThemePartSize function


## -description


Calculates the original size of the part defined by a visual style.


## -parameters




### -param hTheme [in]

Type: <b>HTHEME</b>

Handle to a window's specified theme data. Use <a href="https://msdn.microsoft.com/en-us/library/Bb759821(v=VS.85).aspx">OpenThemeData</a> to create an HTHEME.


### -param hdc [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HDC</a></b>

HDC to select fonts into.


### -param iPartId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the part to calculate the size of. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param iStateId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the state of the part. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param prc [in]

Type: <b>LPCRECT</b>

Pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that contains the rectangle used for the part drawing destination. This parameter may be set to <b>NULL</b>.


### -param arg6 [in]

Type: <b>THEMESIZE</b>

Enumerated type that specifies the type of size to retrieve. See <a href="https://msdn.microsoft.com/en-us/library/Bb759839(v=VS.85).aspx">THEMESIZE</a> for a list of type values.


### -param psz [out]

Type: <b><a href="https://msdn.microsoft.com/8cb0802c-1868-4f3b-8287-c6fb1fa7ab68">SIZE</a>*</b>

Pointer to a <a href="https://msdn.microsoft.com/8cb0802c-1868-4f3b-8287-c6fb1fa7ab68">SIZE</a> structure that receives the dimensions of the specified part.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb773213(v=VS.85).aspx">Property Identifiers</a>
 

 

