---
UID: NF:textserv.ITextServices.TxGetHScroll
title: ITextServices::TxGetHScroll
author: windows-sdk-content
description: Returns horizontal scroll bar information.
old-location: controls\ITextServices_TxGetHScroll.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\windowlessricheditcontrols\windowlessricheditcontrolsreference\windowlessricheditcontrolinterfaces\txgethscroll.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextServices interface [Windows Controls],TxGetHScroll method, ITextServices.TxGetHScroll, ITextServices::TxGetHScroll, TxGetHScroll, TxGetHScroll method [Windows Controls], TxGetHScroll method [Windows Controls],ITextServices interface, _win32_ITextServices_TxGetHScroll, _win32_ITextServices_TxGetHScroll_cpp, controls.ITextServices_TxGetHScroll, controls._win32_ITextServices_TxGetHScroll, textserv/ITextServices::TxGetHScroll
ms.topic: method
req.header: textserv.h
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
req.lib: 
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextServices.TxGetHScroll
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextServices::TxGetHScroll


## -description


Returns horizontal scroll bar information.


## -parameters




### -param plMin

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a>*</b>

The minimum scroll position. 


### -param plMax

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a>*</b>

The maximum scroll position. 


### -param plPos

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a>*</b>

The current scroll position. 


### -param plPage

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LONG</a>*</b>

The view width, in pixels. 


### -param pfEnabled

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a>*</b>

Indicates whether horizontal scrolling is enabled. If <b>TRUE</b>, horizontal scrolling is enabled. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

The method always returns <b>S_OK</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb787617(v=VS.85).aspx">ITextServices</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787609(v=VS.85).aspx">Windowless Rich Edit Controls Overview</a>
 

 

