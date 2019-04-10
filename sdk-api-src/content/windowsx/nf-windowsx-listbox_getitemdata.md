---
UID: NF:windowsx.ListBox_GetItemData
title: ListBox_GetItemData macro (windowsx.h)
author: windows-sdk-content
description: Gets the application-defined value associated with the specified list box item. You can use this macro or send the LB_GETITEMDATA message explicitly.
old-location: controls\ListBox_GetItemData.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listboxes\listboxreference\listboxmacros\listbox_getitemdata.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ListBox_GetItemData, ListBox_GetItemData macro [Windows Controls], _win32_ListBox_GetItemData, _win32_ListBox_GetItemData_cpp, controls.ListBox_GetItemData, controls._win32_ListBox_GetItemData, windowsx/ListBox_GetItemData
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
 - ListBox_GetItemData
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListBox_GetItemData macro


## -description


Gets the application-defined value associated with the specified list box item. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb775202(v=VS.85).aspx">LB_GETITEMDATA</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param index

Type: <b>int</b>

The zero-based index of the item.

