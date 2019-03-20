---
UID: NF:windowsx.ListBox_SetColumnWidth
title: ListBox_SetColumnWidth macro (windowsx.h)
author: windows-sdk-content
description: Sets the width of all columns in a multiple-column list box. You can use this macro or send the LB_SETCOLUMNWIDTH message explicitly.
old-location: controls\ListBox_SetColumnWidth.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listboxes\listboxreference\listboxmacros\listbox_setcolumnwidth.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ListBox_SetColumnWidth, ListBox_SetColumnWidth macro [Windows Controls], _win32_ListBox_SetColumnWidth, _win32_ListBox_SetColumnWidth_cpp, controls.ListBox_SetColumnWidth, controls._win32_ListBox_SetColumnWidth, windowsx/ListBox_SetColumnWidth
ms.topic: macro
req.header: windowsx.h
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
 - Windowsx.h
api_name:
 - ListBox_SetColumnWidth
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListBox_SetColumnWidth macro


## -description


Sets the width of all columns in a multiple-column list box. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761338(v=VS.85).aspx">LB_SETCOLUMNWIDTH</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param cxColumn

Type: <b>int</b>

The width, in pixels, of all columns.

