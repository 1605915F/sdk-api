---
UID: NF:windowsx.ListBox_FindItemData
title: ListBox_FindItemData macro
author: windows-sdk-content
description: Finds the first item in a list box that has the specified item data. You can use this macro or send the LB_FINDSTRING message explicitly.
old-location: controls\ListBox_FindItemData.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\listboxes\listboxreference\listboxmacros\listbox_finditemdata.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ListBox_FindItemData, ListBox_FindItemData macro [Windows Controls], _win32_ListBox_FindItemData, _win32_ListBox_FindItemData_cpp, controls.ListBox_FindItemData, controls._win32_ListBox_FindItemData, windowsx/ListBox_FindItemData
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
 - ListBox_FindItemData
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListBox_FindItemData macro


## -description


Finds the first item in a list box that has the specified item data. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb775187(v=VS.85).aspx">LB_FINDSTRING</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param indexStart

Type: <b>int</b>

The zero-based index of the item before the first item to be searched. When the search reaches the bottom of the list box, it continues searching from the top of the list box back to the item specified by the <i>indexStart</i> parameter. If <i>indexStart</i>  is –1, the entire list box is searched from the beginning.


### -param data

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPARAM</a></b>

The data to find.


## -remarks



For more information, see <a href="https://msdn.microsoft.com/en-us/library/Bb775187(v=VS.85).aspx">LB_FINDSTRING</a>.
	



