---
UID: NF:commctrl.ListView_GetNextItem
title: ListView_GetNextItem macro
author: windows-sdk-content
description: Searches for a list-view item that has the specified properties and bears the specified relationship to a specified item. You can use this macro or send the LVM_GETNEXTITEM message explicitly.
old-location: controls\ListView_GetNextItem.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\listview\macros\listview_getnextitem.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ListView_GetNextItem, ListView_GetNextItem macro [Windows Controls], _win32_ListView_GetNextItem, _win32_ListView_GetNextItem_cpp, commctrl/ListView_GetNextItem, controls.ListView_GetNextItem, controls._win32_ListView_GetNextItem
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ListView_GetNextItem
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListView_GetNextItem macro


## -description


Searches for a list-view item that has the specified properties and bears the specified relationship to a specified item. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761057(v=VS.85).aspx">LVM_GETNEXTITEM</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">HWND</a></b>

A handle to the list-view control. 


### -param i

Type: <b>int</b>

The index of the item with which to begin the search, or -1 to find the first item that matches the specified flags. The specified item itself is excluded from the search. 


### -param flags

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

The geometric relation of the requested item to the specified item and, if specified, the state of the requested item. For a list of possible values, see the description of the 
					<i>lParam</i> parameter in the <a href="https://msdn.microsoft.com/en-us/library/Bb761057(v=VS.85).aspx">LVM_GETNEXTITEM</a> message. If an item does not have all of the specified state flags set, the search continues with the next item. 

