---
UID: NF:commctrl.TreeView_GetItemState
title: TreeView_GetItemState macro
author: windows-sdk-content
description: Retrieves some or all of a tree-view item's state attributes. You can use this macro or send the TVM_GETITEMSTATE message explicitly.
old-location: controls\TreeView_GetItemState.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\macros\treeview_getitemstate.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TreeView_GetItemState, TreeView_GetItemState macro [Windows Controls], _win32_TreeView_GetItemState, _win32_TreeView_GetItemState_cpp, commctrl/TreeView_GetItemState, controls.TreeView_GetItemState, controls._win32_TreeView_GetItemState
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
 - TreeView_GetItemState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TreeView_GetItemState macro


## -description


Retrieves some or all of a tree-view item's state attributes. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb773614(v=VS.85).aspx">TVM_GETITEMSTATE</a> message explicitly. 


## -parameters




### -param hwndTV

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the tree-view control. 


### -param hti

Type: <b>HTREEITEM</b>

Handle to the item. 


### -param mask

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Mask used to specify the states to query for. It is equivalent to the <b>stateMask</b> member of <a href="https://msdn.microsoft.com/en-us/library/Bb773459(v=VS.85).aspx">TVITEMEX</a>. 

