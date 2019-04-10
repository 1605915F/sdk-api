---
UID: NF:commctrl.TreeView_GetRoot
title: TreeView_GetRoot macro (commctrl.h)
author: windows-sdk-content
description: Retrieves the topmost or very first item of the tree-view control. You can use this macro, or you can explicitly send the TVM_GETNEXTITEM message with the TVGN_ROOT flag.
old-location: controls\TreeView_GetRoot.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\macros\treeview_getroot.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: TreeView_GetRoot, TreeView_GetRoot macro [Windows Controls], _win32_TreeView_GetRoot, _win32_TreeView_GetRoot_cpp, commctrl/TreeView_GetRoot, controls.TreeView_GetRoot, controls._win32_TreeView_GetRoot
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
 - TreeView_GetRoot
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TreeView_GetRoot macro


## -description


Retrieves the topmost or very first item of the tree-view control. You can use this macro, or you can explicitly send the <a href="https://msdn.microsoft.com/en-us/library/Bb773622(v=VS.85).aspx">TVM_GETNEXTITEM</a> message with the TVGN_ROOT flag. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the tree-view control. 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb773861(v=VS.85).aspx">TreeView_GetNextItem</a>
 

 

