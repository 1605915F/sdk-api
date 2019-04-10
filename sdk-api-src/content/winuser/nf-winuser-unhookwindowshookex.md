---
UID: NF:winuser.UnhookWindowsHookEx
title: UnhookWindowsHookEx function (winuser.h)
author: windows-sdk-content
description: Removes a hook procedure installed in a hook chain by the SetWindowsHookEx function.
old-location: winmsg\unhookwindowshookex.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\hooks\hookreference\hookfunctions\unhookwindowshookex.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: UnhookWindowsHookEx, UnhookWindowsHookEx function [Windows and Messages], _win32_UnhookWindowsHookEx, _win32_unhookwindowshookex_cpp, winmsg.unhookwindowshookex, winui._win32_unhookwindowshookex, winuser/UnhookWindowsHookEx
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
 - UnhookWindowsHookEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# UnhookWindowsHookEx function


## -description


Removes a hook procedure installed in a hook chain by the <a href="https://msdn.microsoft.com/en-us/library/ms644990(v=VS.85).aspx">SetWindowsHookEx</a> function. 


## -parameters




### -param hhk [in]

Type: <b>HHOOK</b>

A handle to the hook to be removed. This parameter is a hook handle obtained by a previous call to <a href="https://msdn.microsoft.com/en-us/library/ms644990(v=VS.85).aspx">SetWindowsHookEx</a>. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The hook procedure can be in the state of being called by another thread even after <b>UnhookWindowsHookEx</b> returns. If the hook procedure is not being called concurrently, the hook procedure is removed immediately before <b>UnhookWindowsHookEx</b> returns. 


#### Examples

For an example, see <a href="https://msdn.microsoft.com/en-us/library/ms644960(v=VS.85).aspx">Monitoring System Events</a>.

<div class="code"></div>



## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632589(v=VS.85).aspx">Hooks</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms644990(v=VS.85).aspx">SetWindowsHookEx</a>
 

 

