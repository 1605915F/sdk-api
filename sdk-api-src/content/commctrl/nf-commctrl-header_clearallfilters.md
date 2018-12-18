---
UID: NF:commctrl.Header_ClearAllFilters
title: Header_ClearAllFilters macro
author: windows-sdk-content
description: Clears all of the filters for a given header control. You can use this macro or send the HDM_CLEARFILTER message explicitly.
old-location: controls\Header_ClearAllFilters.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\header\macros\header_clearallfilters.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Header_ClearAllFilters, Header_ClearAllFilters macro [Windows Controls], _win32_Header_ClearAllFilters, _win32_Header_ClearAllFilters_cpp, commctrl/Header_ClearAllFilters, controls.Header_ClearAllFilters, controls._win32_Header_ClearAllFilters
ms.topic: macro
req.header: commctrl.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Commctrl.h
api_name:
 - Header_ClearAllFilters
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# Header_ClearAllFilters macro


## -description


Clears all of the filters for a given header control. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb775306(v=VS.85).aspx">HDM_CLEARFILTER</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the header control. 


## -remarks



When all the filters are cleared, the <a href="https://msdn.microsoft.com/en-us/library/Bb775277(v=VS.85).aspx">HDN_FILTERCHANGE</a> notification will be sent only once. 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb775377(v=VS.85).aspx">Header_ClearFilter</a>
 

 

