---
UID: NS:winuser.tagLASTINPUTINFO
title: LASTINPUTINFO (winuser.h)
author: windows-sdk-content
description: Contains the time of the last input.
old-location: inputdev\lastinputinfo.htm
tech.root: inputdev
ms.assetid: VS|winui|~\winui\windowsuserinterface\userinput\keyboardinput\keyboardinputreference\keyboardinputstructures\lastinputinfo.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PLASTINPUTINFO, LASTINPUTINFO, LASTINPUTINFO structure [Keyboard and Mouse Input], PLASTINPUTINFO, PLASTINPUTINFO structure pointer [Keyboard and Mouse Input], _win32_LASTINPUTINFO_str, _win32_lastinputinfo_str_cpp, inputdev.lastinputinfo, winui._win32_lastinputinfo_str, winuser/LASTINPUTINFO, winuser/PLASTINPUTINFO"
ms.topic: struct
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Winuser.h
api_name:
 - LASTINPUTINFO
product: Windows
targetos: Windows
req.typenames: LASTINPUTINFO, *PLASTINPUTINFO
req.redist: 
---

# LASTINPUTINFO structure


## -description


Contains the time of the last input.


## -struct-fields




### -field cbSize

Type: <b>UINT</b>

The size of the structure, in bytes. This member must be set to <code>sizeof(LASTINPUTINFO)</code>. 


### -field dwTime

Type: <b>DWORD</b>

The tick count when the last input event was received. 


## -remarks



This function is useful for input idle detection. For more information on tick counts, see <a href="https://msdn.microsoft.com/22201c82-a49a-4972-9f49-6baf6d23a1ea">GetTickCount</a>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms646302(v=VS.85).aspx">GetLastInputInfo</a>



<a href="https://msdn.microsoft.com/22201c82-a49a-4972-9f49-6baf6d23a1ea">GetTickCount</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645530(v=VS.85).aspx">Keyboard Input</a>



<b>Reference</b>
 

 

