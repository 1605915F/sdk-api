---
UID: NF:commctrl.TreeView_GetItemRect
title: TreeView_GetItemRect macro
author: windows-sdk-content
description: Retrieves the bounding rectangle for a tree-view item and indicates whether the item is visible. You can use this macro or send the TVM_GETITEMRECT message explicitly.
old-location: controls\TreeView_GetItemRect.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\macros\treeview_getitemrect.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TreeView_GetItemRect, TreeView_GetItemRect macro [Windows Controls], _win32_TreeView_GetItemRect, _win32_TreeView_GetItemRect_cpp, commctrl/TreeView_GetItemRect, controls.TreeView_GetItemRect, controls._win32_TreeView_GetItemRect
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
 - TreeView_GetItemRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TreeView_GetItemRect macro


## -description


Retrieves the bounding rectangle for a tree-view item and indicates whether the item is visible. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb773610(v=VS.85).aspx">TVM_GETITEMRECT</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the tree-view control. 


### -param hitem

Type: <b>HTREEITEM</b>

Handle to the tree-view item. 


### -param prc

Type: <b>LPRECT</b>

Pointer to a <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that receives the bounding rectangle. The coordinates are relative to the upper-left corner of the tree-view control. 


### -param code

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

Value specifying the portion of the item for which to retrieve the bounding rectangle. If this parameter is <b>TRUE</b>, the bounding rectangle includes only the text of the item. Otherwise, it includes the entire line that the item occupies in the tree-view control. 

