---
UID: NF:commctrl.Header_Layout
title: Header_Layout macro (commctrl.h)
author: windows-sdk-content
description: Retrieves the correct size and position of a header control within the parent window. You can use this macro or send the HDM_LAYOUT message explicitly.
old-location: controls\Header_Layout.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\header\macros\header_layout.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Header_Layout, Header_Layout macro [Windows Controls], _win32_Header_Layout, _win32_Header_Layout_cpp, commctrl/Header_Layout, controls.Header_Layout, controls._win32_Header_Layout
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
 - Header_Layout
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# Header_Layout macro


## -description


Retrieves the correct size and position of a header control within the parent window. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb775353(v=VS.85).aspx">HDM_LAYOUT</a> message explicitly. 


## -parameters




### -param hwndHD [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the header control. 


### -param playout [out]

Type: <b>LPHDLAYOUT</b>

A pointer to an <a href="https://msdn.microsoft.com/en-us/library/Bb775249(v=VS.85).aspx">HDLAYOUT</a> structure. The 
					<b>prc</b> member specifies the coordinates of a rectangle, and the 
					<b>pwpos</b> member receives the size and position for the header control within the rectangle. 


## -remarks



The <b>Header_Layout</b> macro is defined as follows: 

<pre class="syntax" xml:space="preserve"><code>#define Header_Layout(hwndHD, playout) \

    (BOOL)SendMessage((hwndHD), HDM_LAYOUT, 0, \

    (LPARAM)(LPHDLAYOUT)(playout))</code></pre>


