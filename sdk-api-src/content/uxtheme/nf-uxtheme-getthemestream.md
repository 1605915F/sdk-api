---
UID: NF:uxtheme.GetThemeStream
title: GetThemeStream function
author: windows-sdk-content
description: Retrieves a data stream corresponding to a specified theme, starting from a specified part, state, and property.
old-location: controls\GetThemeStream.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\userex\functions\getthemestream.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetThemeStream, GetThemeStream function [Windows Controls], controls.GetThemeStream, controls.inet_GetThemeStream, inet_GetThemeStream, inet_GetThemeStream_cpp, uxtheme/GetThemeStream
ms.topic: function
req.header: uxtheme.h
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
 - GetThemeStream
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetThemeStream function


## -description


Retrieves a data stream corresponding to a specified theme, starting from a specified part, state, and property.


## -parameters




### -param hTheme [in]

Type: <b>HTHEME</b>

Handle to the theme from which the stream will be retrieved.


### -param iPartId [in]

Type: <b>int</b>

Specifies the part to retrieve a stream from. See <a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>.


### -param iStateId [in]

Type: <b>int</b>

Specifies the state of the part.


### -param iPropId [in]

Type: <b>int</b>

Specifies the property to retrieve.


### -param ppvStream [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">VOID</a>**</b>

Address of a pointer that receives the stream.


### -param pcbStream [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a>*</b>

Pointer that receives the length, in bytes, of the stream received by <i>ppvStream</i>.


### -param hInst [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HINSTANCE</a></b>

If <i>iPropId</i> is TMT_STREAM, this value is <b>NULL</b>. If <i>iPropId</i> is TMT_DISKSTREAM, this value is the HINSTANCE of a loaded styles file.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<b>Windows 8:</b> In high contrast mode, the data stream retrieved by this function is not valid after the <i>hTheme</i> theme handle is closed.


The data stream retrieved by this function is not a copy; do not delete or close the data stream after using it.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb773210(v=VS.85).aspx">Parts and States</a>
 

 

