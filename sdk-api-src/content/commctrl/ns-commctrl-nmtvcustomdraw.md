---
UID: NS:commctrl.tagNMTVCUSTOMDRAW
title: NMTVCUSTOMDRAW (commctrl.h)
author: windows-sdk-content
description: Contains information specific to an NM_CUSTOMDRAW (tree view) notification code sent by a tree-view control.
old-location: controls\NMTVCUSTOMDRAW.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\treeview\structures\nmtvcustomdraw.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPNMTVCUSTOMDRAW, LPNMTVCUSTOMDRAW, LPNMTVCUSTOMDRAW structure pointer [Windows Controls], NMTVCUSTOMDRAW, NMTVCUSTOMDRAW structure [Windows Controls], _win32_NMTVCUSTOMDRAW, _win32_NMTVCUSTOMDRAW_cpp, commctrl/LPNMTVCUSTOMDRAW, commctrl/NMTVCUSTOMDRAW, controls.NMTVCUSTOMDRAW, controls._win32_NMTVCUSTOMDRAW"
ms.topic: struct
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
 - NMTVCUSTOMDRAW
product: Windows
targetos: Windows
req.typenames: NMTVCUSTOMDRAW, *LPNMTVCUSTOMDRAW
req.redist: 
ms.custom: 19H1
---

# NMTVCUSTOMDRAW structure


## -description


Contains information specific to an <a href="https://msdn.microsoft.com/en-us/library/Bb773470(v=VS.85).aspx">NM_CUSTOMDRAW (tree view)</a> notification code sent by a tree-view control. 


## -struct-fields




### -field nmcd

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb775483(v=VS.85).aspx">NMCUSTOMDRAW</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb775483(v=VS.85).aspx">NMCUSTOMDRAW</a> structure that contains general custom draw information. 


### -field clrText

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">COLORREF</a></b>


<a href="https://msdn.microsoft.com/b87d3de2-7a13-44ef-8253-c6851a75fa54">COLORREF</a> value representing the color that will be used to display text foreground in the tree-view control. 


### -field clrTextBk

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">COLORREF</a></b>


<a href="https://msdn.microsoft.com/b87d3de2-7a13-44ef-8253-c6851a75fa54">COLORREF</a> value representing the color that will be used to display text background in the tree-view control. 


### -field iLevel

Type: <b>int</b>


<a href="https://msdn.microsoft.com/1B524A91-B433-4968-9546-8A6AFB67E89C">Version 4.71</a>. Zero-based level of the item being drawn. The root item is at level zero, a child of the root item is at level one, and so on. 

