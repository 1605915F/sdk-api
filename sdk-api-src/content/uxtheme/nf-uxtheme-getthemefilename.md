---
UID: NF:uxtheme.GetThemeFilename
title: GetThemeFilename function (uxtheme.h)
author: windows-sdk-content
description: Retrieves the value of a filename property.
old-location: controls\GetThemeFilename.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\userex\functions\getthemefilename.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetThemeFilename, GetThemeFilename function [Windows Controls], controls.GetThemeFilename, controls.inet_GetThemeFilename, inet_GetThemeFilename, inet_GetThemeFilename_cpp, uxtheme/GetThemeFilename
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
 - GetThemeFilename
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetThemeFilename function


## -description


Retrieves the value of a filename property.


## -parameters




### -param hTheme [in]

Type: <b>HTHEME</b>

Handle to a window's specified theme data. Use <a href="https://msdn.microsoft.com/en-us/library/Bb759821(v=VS.85).aspx">OpenThemeData</a> to create an HTHEME.


### -param iPartId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the part that contains the filename property. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>. 


### -param iStateId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the state of the part. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param iPropId [in]

Type: <b>int</b>

Value of type <b>int</b> that specifies the property to retrieve. For a list of possible values, see <a href="https://msdn.microsoft.com/en-us/library/Bb773213(v=VS.85).aspx">Property Identifiers</a>.


### -param pszThemeFileName [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPWSTR</a></b>

Pointer to a buffer that receives the retrieved file name.


### -param cchMaxBuffChars [in]

Type: <b>int</b>

Value of type <b>int</b> that receives the maximum number of characters in the file name


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb773213(v=VS.85).aspx">Property Identifiers</a>
 

 

