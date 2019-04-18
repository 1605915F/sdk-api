---
UID: NF:dwmapi.DwmIsCompositionEnabled
title: DwmIsCompositionEnabled function (dwmapi.h)
author: windows-sdk-content
description: Obtains a value that indicates whether Desktop Window Manager (DWM) composition is enabled. Applications on machines running Windows 7 or earlier can listen for composition state changes by handling the WM_DWMCOMPOSITIONCHANGED notification.
old-location: dwm\dwmiscompositionenabled.htm
tech.root: dwm
ms.assetid: VS|winui|~\winui\desktopwindowmanager\reference\functions\dwmiscompositionenabled.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DwmIsCompositionEnabled, DwmIsCompositionEnabled function [Desktop Window Manager], _udwm_dwmiscompositionenabled, _udwm_dwmiscompositionenabled_cpp, dwm.dwmiscompositionenabled, dwmapi/DwmIsCompositionEnabled, winui._udwm_dwmiscompositionenabled
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
 - API-MS-Win-dwmapi-l1-1-0.dll
 - Ext-Ms-Win-DwmAPI-Ext-L1-1-0.dll
api_name:
 - DwmIsCompositionEnabled
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# DwmIsCompositionEnabled function


## -description


Obtains a value that indicates whether Desktop Window Manager (DWM) composition is enabled. Applications on machines running Windows 7 or earlier can listen for composition state changes by handling the <a href="https://msdn.microsoft.com/en-us/library/Dd388199(v=VS.85).aspx">WM_DWMCOMPOSITIONCHANGED</a> notification.


## -parameters




### -param pfEnabled [out]

A pointer to a value that, when this function returns successfully, receives <b>TRUE</b> if DWM composition is enabled; otherwise, <b>FALSE</b>.

                        

<div class="alert"><b>Note</b>  As of Windows 8, DWM composition is always enabled. If an app declares Windows 8 compatibility in their manifest, this function will receive a value of <b>TRUE</b> through <i>pfEnabled</i>. If no such manifest entry is found, Windows 8 compatibility is not assumed and this function receives a value of <b>FALSE</b> through <i>pfEnabled</i>. This is done so that older programs that interpret a value of <b>TRUE</b> to imply that high contrast mode is off can continue to make the correct decisions about rendering their images. (Note that this is a bad practice—you should use the <a href="https://msdn.microsoft.com/9b99465c-e12d-413c-8e69-b46b52f2f11f">SystemParametersInfo</a> function with the <b>SPI_GETHIGHCONTRAST</b> flag to determine the state of high contrast mode.)</div>
<div> </div>
For more information, see <a href="http://go.microsoft.com/fwlink/p/?linkid=389859">Supporting High Contrast Themes</a>.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



