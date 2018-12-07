---
UID: NF:commctrl.TreeView_GetToolTips
title: TreeView_GetToolTips macro
author: windows-sdk-content
description: Retrieves the handle to the child tooltip control used by a tree-view control. You can use this macro or send the TVM_GETTOOLTIPS message explicitly.
old-location: controls\TreeView_GetToolTips.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\treeview\macros\treeview_gettooltips.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TreeView_GetToolTips, TreeView_GetToolTips macro [Windows Controls], _win32_TreeView_GetToolTips, _win32_TreeView_GetToolTips_cpp, commctrl/TreeView_GetToolTips, controls.TreeView_GetToolTips, controls._win32_TreeView_GetToolTips
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
 - TreeView_GetToolTips
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TreeView_GetToolTips macro


## -description


Retrieves the handle to the child tooltip control used by a tree-view control. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb773729(v=VS.85).aspx">TVM_GETTOOLTIPS</a> message explicitly. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">HWND</a></b>

Handle to a tree-view control. 


## -remarks



When created, tree-view controls automatically create a child tooltip control. To prevent a tree-view control from using tooltips, create the control with the <a href="https://msdn.microsoft.com/en-us/library/Bb760013(v=VS.85).aspx">TVS_NOTOOLTIPS</a> style. 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb760133(v=VS.85).aspx">TreeView_SetToolTips</a>
 

 

