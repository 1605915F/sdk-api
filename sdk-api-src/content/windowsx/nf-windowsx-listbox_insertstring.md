---
UID: NF:windowsx.ListBox_InsertString
title: ListBox_InsertString macro (windowsx.h)
author: windows-sdk-content
description: Adds a string to a list box at the specified location. You can use this macro or send the LB_INSERTSTRING message explicitly.
old-location: controls\ListBox_InsertString.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listboxes\listboxreference\listboxmacros\listbox_insertstring.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ListBox_InsertString, ListBox_InsertString macro [Windows Controls], _win32_ListBox_InsertString, _win32_ListBox_InsertString_cpp, controls.ListBox_InsertString, controls._win32_ListBox_InsertString, windowsx/ListBox_InsertString
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
 - ListBox_InsertString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListBox_InsertString macro


## -description


Adds a string to a list box at the specified location. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761321(v=VS.85).aspx">LB_INSERTSTRING</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param index

Type: <b>int</b>

The zero-based index at which to insert the string, or –1 to add it to the end of the list. 


### -param lpsz

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCSTR</a></b>

The string to add.


## -remarks



For more information, see <a href="https://msdn.microsoft.com/en-us/library/Bb761321(v=VS.85).aspx">LB_INSERTSTRING</a>.
	



