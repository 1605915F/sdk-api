---
UID: NF:dwmapi.DwmGetWindowAttribute
title: DwmGetWindowAttribute function
author: windows-sdk-content
description: Retrieves the current value of a specified attribute applied to a window.
old-location: dwm\dwmgetwindowattribute.htm
tech.root: dwm
ms.assetid: VS|winui|~\winui\desktopwindowmanager\reference\functions\dwmgetwindowattribute.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DwmGetWindowAttribute, DwmGetWindowAttribute function [Desktop Window Manager], _udwm_dwmgetwindowattribute, _udwm_dwmgetwindowattribute_cpp, dwm.dwmgetwindowattribute, dwmapi/DwmGetWindowAttribute, winui._udwm_dwmgetwindowattribute
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: dwmapi.h
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
req.lib: Dwmapi.lib
req.dll: Dwmapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Dwmapi.dll
api_name:
 - DwmGetWindowAttribute
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DwmGetWindowAttribute function


## -description


Retrieves the current value of a specified attribute applied to a window.


## -parameters




### -param hwnd

The handle to the window from which the attribute data is retrieved.


### -param dwAttribute

The attribute to retrieve, specified as a <a href="https://msdn.microsoft.com/en-us/library/Aa969530(v=VS.85).aspx">DWMWINDOWATTRIBUTE</a> value.


### -param pvAttribute [out]

A pointer to a value that, when this function returns successfully, receives the current value of the attribute. The type of the retrieved value depends on the value of the <i>dwAttribute</i> parameter.


### -param cbAttribute

The size of the <a href="https://msdn.microsoft.com/en-us/library/Aa969530(v=VS.85).aspx">DWMWINDOWATTRIBUTE</a> value being retrieved. The size is dependent on the type of the <i>pvAttribute</i> parameter.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa969524(v=VS.85).aspx">DwmSetWindowAttribute</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa969538(v=VS.85).aspx">Enable and Control DWM Composition</a>
 

 

