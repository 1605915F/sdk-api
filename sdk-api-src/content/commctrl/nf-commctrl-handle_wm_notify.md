---
UID: NF:commctrl.HANDLE_WM_NOTIFY
title: HANDLE_WM_NOTIFY macro (commctrl.h)
author: windows-sdk-content
description: Calls a function that processes the WM_NOTIFY message.
old-location: controls\HANDLE_WM_NOTIFY.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\common\macros\handle_wm_notify.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: HANDLE_WM_NOTIFY, HANDLE_WM_NOTIFY macro [Windows Controls], _win32_HANDLE_WM_NOTIFY, _win32_HANDLE_WM_NOTIFY_cpp, commctrl/HANDLE_WM_NOTIFY, controls.HANDLE_WM_NOTIFY, controls._win32_HANDLE_WM_NOTIFY
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
 - HANDLE_WM_NOTIFY
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# HANDLE_WM_NOTIFY macro


## -description


Calls a function that processes the <a href="https://msdn.microsoft.com/en-us/library/Bb775583(v=VS.85).aspx">WM_NOTIFY</a> message. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the window that received <a href="https://msdn.microsoft.com/en-us/library/Bb775583(v=VS.85).aspx">WM_NOTIFY</a>. 


### -param wParam

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">WPARAM</a></b>

The first parameter of <a href="https://msdn.microsoft.com/en-us/library/Bb775583(v=VS.85).aspx">WM_NOTIFY</a>. 


### -param lParam

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPARAM</a></b>

The second parameter of <a href="https://msdn.microsoft.com/en-us/library/Bb775583(v=VS.85).aspx">WM_NOTIFY</a>. 


### -param fn

Type: <b>function</b>

The function that is to process <a href="https://msdn.microsoft.com/en-us/library/Bb775583(v=VS.85).aspx">WM_NOTIFY</a>. 


## -remarks



The <b>HANDLE_WM_NOTIFY</b> macro is defined as follows. 

<pre class="syntax" xml:space="preserve"><code>#define HANDLE_WM_NOTIFY(hwnd, wParam, lParam, fn) \ 

    (fn)((hwnd), (int)(wParam), (NMHDR*)(lParam))</code></pre>
The macro can be used inside a dialog window procedure to simplify the calling of an application-defined function that requires an <a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a> parameter.



