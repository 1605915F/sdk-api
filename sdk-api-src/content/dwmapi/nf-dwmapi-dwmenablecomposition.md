---
UID: NF:dwmapi.DwmEnableComposition
title: DwmEnableComposition function
author: windows-sdk-content
description: Enables or disables Desktop Window Manager (DWM) composition.
old-location: dwm\dwmenablecomposition.htm
tech.root: dwm
ms.assetid: VS|winui|~\winui\desktopwindowmanager\reference\functions\dwmenablecomposition.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DwmEnableComposition, DwmEnableComposition function [Desktop Window Manager], _udwm_dwmenablecomposition, _udwm_dwmenablecomposition_cpp, dwm.dwmenablecomposition, dwmapi/DwmEnableComposition, winui._udwm_dwmenablecomposition
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
 - DwmEnableComposition
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DwmEnableComposition function


## -description


Enables or disables Desktop Window Manager (DWM) composition.
        
            
<div class="alert"><b>Note</b>  This function is deprecated as of Windows 8. DWM can no longer be programmatically disabled.</div><div> </div>

## -parameters




### -param uCompositionAction

<b>DWM_EC_ENABLECOMPOSITION</b> to enable DWM composition; <b>DWM_EC_DISABLECOMPOSITION</b> to disable composition.
                        

<div class="alert"><b>Note</b>  As of Windows 8, calling this function with <b>DWM_EC_DISABLECOMPOSITION</b> has no effect. However, the function will still return a success code.</div>
<div> </div>

## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Disabling DWM composition disables it for the entire desktop. DWM composition will be automatically enabled when all processes that have disabled composition have called <b>DwmEnableComposition</b> to enable it or have been terminated. The <a href="https://msdn.microsoft.com/en-us/library/Dd388199(v=VS.85).aspx">WM_DWMCOMPOSITIONCHANGED</a> notification is sent whenever DWM composition is enabled or disabled.


#### Examples

The following code example disables DWM composition.


```cpp

...
HRESULT hr = S_OK;

// Disable DWM Composition 
hr = DwmEnableComposition(DWM_EC_DISABLECOMPOSITION);
if (SUCCEEDED(hr))
{
   // ...
}
...
```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa969538(v=VS.85).aspx">Enable and Control DWM Composition</a>
 

 

