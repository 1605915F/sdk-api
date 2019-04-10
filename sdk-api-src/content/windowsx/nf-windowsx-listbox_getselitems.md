---
UID: NF:windowsx.ListBox_GetSelItems
title: ListBox_GetSelItems macro (windowsx.h)
author: windows-sdk-content
description: Gets the indexes of selected items in a multiple-selection list box. You can use this macro or send the LB_GETSELITEMS message explicitly.
old-location: controls\ListBox_GetSelItems.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listboxes\listboxreference\listboxmacros\listbox_getselitems.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ListBox_GetSelItems, ListBox_GetSelItems macro [Windows Controls], _win32_ListBox_GetSelItems, _win32_ListBox_GetSelItems_cpp, controls.ListBox_GetSelItems, controls._win32_ListBox_GetSelItems, windowsx/ListBox_GetSelItems
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
 - ListBox_GetSelItems
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListBox_GetSelItems macro


## -description


Gets the indexes of selected items in a multiple-selection list box. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761311(v=VS.85).aspx">LB_GETSELITEMS</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param cItems

Type: <b>int</b>

The maximum number of selected items whose item numbers are to be placed in the buffer.


### -param lpItems

Type: <b>int*</b>

A pointer to a buffer large enough for the number of integers specified by <i>cItems</i>. 

