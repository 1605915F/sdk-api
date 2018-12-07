---
UID: NS:winuser.tagCBTACTIVATESTRUCT
title: tagCBTACTIVATESTRUCT
author: windows-sdk-content
description: Contains information passed to a WH_CBT hook procedure, CBTProc, before a window is activated.
old-location: winmsg\cbtactivatestruct.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\hooks\hookreference\hookstructures\cbtactivatestruct.htm
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: "*LPCBTACTIVATESTRUCT, CBTACTIVATESTRUCT, CBTACTIVATESTRUCT structure [Windows and Messages], LPCBTACTIVATESTRUCT, LPCBTACTIVATESTRUCT structure pointer [Windows and Messages], _win32_CBTACTIVATESTRUCT_str, _win32_cbtactivatestruct_str_cpp, tagCBTACTIVATESTRUCT, winmsg.cbtactivatestruct, winui._win32_cbtactivatestruct_str, winuser/CBTACTIVATESTRUCT, winuser/LPCBTACTIVATESTRUCT"
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - CBTACTIVATESTRUCT
product: Windows
targetos: Windows
req.typenames: CBTACTIVATESTRUCT, *LPCBTACTIVATESTRUCT
req.redist: 
---

# tagCBTACTIVATESTRUCT structure


## -description


Contains information passed to a <b>WH_CBT</b> hook procedure, <a href="https://msdn.microsoft.com/en-us/library/ms644977(v=VS.85).aspx">CBTProc</a>, before a window is activated. 


## -struct-fields




### -field fMouse

Type: <b>BOOL</b>

This member is <b>TRUE</b> if a mouse click is causing the activation or <b>FALSE</b> if it is not. 


### -field hWndActive

Type: <b>HWND</b>

A handle to the active window. 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms644977(v=VS.85).aspx">CBTProc</a>



<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632589(v=VS.85).aspx">Hooks</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms644990(v=VS.85).aspx">SetWindowsHookEx</a>
 

 

