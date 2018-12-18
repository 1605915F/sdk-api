---
UID: NF:winuser.GetWindowInfo
title: GetWindowInfo function
author: windows-sdk-content
description: Retrieves information about the specified window.
old-location: winmsg\getwindowinfo.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windows\windowreference\windowfunctions\getwindowinfo.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetWindowInfo, GetWindowInfo function [Windows and Messages], _win32_GetWindowInfo, _win32_getwindowinfo_cpp, winmsg.getwindowinfo, winui._win32_getwindowinfo, winuser/GetWindowInfo
ms.topic: function
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
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
 - Ext-MS-Win-NTUser-Window-l1-1-0.dll
 - Ext-MS-Win-NTUser-Window-l1-1-1.dll
 - Ext-MS-Win-NTUser-Window-l1-1-2.dll
 - Ext-MS-Win-RTCore-NTUser-Window-Ext-l1-1-0.dll
 - minuser.dll
 - ext-ms-win-ntuser-window-l1-1-3.dll
 - Ext-MS-Win-NTUser-Window-L1-1-4.dll
api_name:
 - GetWindowInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetWindowInfo function


## -description


Retrieves information about the specified window.


## -parameters




### -param hwnd [in]

Type: <b>HWND</b>

A handle to the window whose information is to be retrieved. 


### -param pwi [in, out]

Type: <b>PWINDOWINFO</b>

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms632610(v=VS.85).aspx">WINDOWINFO</a> structure to receive the information. Note that you must set the <b>cbSize</b> member to <code>sizeof(WINDOWINFO)</code> before calling this function. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. 

To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. 




## -see-also




<b>Conceptual</b>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632610(v=VS.85).aspx">WINDOWINFO</a>



<a href="https://msdn.microsoft.com/en-us/library/ms632595(v=VS.85).aspx">Windows</a>
 

 

