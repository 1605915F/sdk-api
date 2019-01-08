---
UID: NF:commctrl.TreeView_GetISearchString
title: TreeView_GetISearchString macro
author: windows-sdk-content
description: Retrieves the incremental search string for a tree-view control. The tree-view control uses the incremental search string to select an item based on characters typed by the user. You can use this macro or send the TVM_GETISEARCHSTRING message explicitly.
old-location: controls\TreeView_GetISearchString.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\macros\treeview_getisearchstring.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TreeView_GetISearchString, TreeView_GetISearchString macro [Windows Controls], _win32_TreeView_GetISearchString, _win32_TreeView_GetISearchString_cpp, commctrl/TreeView_GetISearchString, controls.TreeView_GetISearchString, controls._win32_TreeView_GetISearchString
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
 - TreeView_GetISearchString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TreeView_GetISearchString macro


## -description


Retrieves the incremental search string for a tree-view control. The tree-view control uses the incremental search string to select an item based on characters typed by the user. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb773592(v=VS.85).aspx">TVM_GETISEARCHSTRING</a> message explicitly. 


## -parameters




### -param hwndTV

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the tree-view control. 


### -param lpsz

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPTSTR</a></b>

Pointer to the buffer that receives the incremental search string. 


## -remarks



<b>Security Warning:  </b>Using this macro incorrectly might compromise the security of your program. You must allocate a large enough buffer to hold the string. First call the macro passing <b>NULL</b> in <i>lpsz</i>. This returns the number of characters, excluding <b>NULL</b>, that are required. Then call the macro a second time to retrieve the string.  You should review <a href="https://msdn.microsoft.com/en-us/library/Bb773171(v=VS.85).aspx">Security Considerations: Microsoft Windows Controls</a> before continuing.

If the tree-view control is not in incremental search mode, the return value is zero. 



