---
UID: NF:windowsx.ListBox_GetTextLen
title: ListBox_GetTextLen macro
author: windows-sdk-content
description: Gets the length of a string in a list box. You can use this macro or send the LB_GETTEXTLEN message explicitly.
old-location: controls\ListBox_GetTextLen.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\listboxes\listboxreference\listboxmacros\listbox_gettextlen.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ListBox_GetTextLen, ListBox_GetTextLen macro [Windows Controls], _win32_ListBox_GetTextLen, _win32_ListBox_GetTextLen_cpp, controls.ListBox_GetTextLen, controls._win32_ListBox_GetTextLen, windowsx/ListBox_GetTextLen
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ListBox_GetTextLen
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListBox_GetTextLen macro


## -description


Gets the length of a string in a list box.  You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761315(v=VS.85).aspx">LB_GETTEXTLEN</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param index

Type: <b>int</b>

The zero-based index of the item.


## -remarks



For more information, see <a href="https://msdn.microsoft.com/en-us/library/Bb761315(v=VS.85).aspx">LB_GETTEXTLEN</a>.
	



