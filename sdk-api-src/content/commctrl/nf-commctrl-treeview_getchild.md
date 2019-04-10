---
UID: NF:commctrl.TreeView_GetChild
title: TreeView_GetChild macro (commctrl.h)
author: windows-sdk-content
description: Retrieves the first child item of the specified tree-view item. You can use this macro, or you can explicitly send the TVM_GETNEXTITEM message with the TVGN_CHILD flag.
old-location: controls\TreeView_GetChild.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\macros\treeview_getchild.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: TreeView_GetChild, TreeView_GetChild macro [Windows Controls], _win32_TreeView_GetChild, _win32_TreeView_GetChild_cpp, commctrl/TreeView_GetChild, controls.TreeView_GetChild, controls._win32_TreeView_GetChild
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
 - TreeView_GetChild
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TreeView_GetChild macro


## -description


Retrieves the first child item of the specified tree-view item. You can use this macro, or you can explicitly send the <a href="https://msdn.microsoft.com/en-us/library/Bb773622(v=VS.85).aspx">TVM_GETNEXTITEM</a> message with the TVGN_CHILD flag. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the tree-view control. 


### -param hitem

Type: <b>HTREEITEM</b>

Handle to a tree-view item. 


## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb773861(v=VS.85).aspx">TreeView_GetNextItem</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb773867(v=VS.85).aspx">TreeView_GetNextSibling</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb773872(v=VS.85).aspx">TreeView_GetParent</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb773875(v=VS.85).aspx">TreeView_GetPrevSibling</a>
 

 

