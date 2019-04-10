---
UID: NF:commctrl.ListView_GetCheckState
title: ListView_GetCheckState macro (commctrl.h)
author: windows-sdk-content
description: Determines if an item in a list-view control is selected. This should be used only for list-view controls that have the LVS_EX_CHECKBOXES style.
old-location: controls\ListView_GetCheckState.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listview\macros\listview_getcheckstate.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ListView_GetCheckState, ListView_GetCheckState macro [Windows Controls], _win32_ListView_GetCheckState, _win32_ListView_GetCheckState_cpp, commctrl/ListView_GetCheckState, controls.ListView_GetCheckState, controls._win32_ListView_GetCheckState
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
 - ListView_GetCheckState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ListView_GetCheckState macro


## -description


Determines if an item in a list-view control is selected. This should be used only for list-view controls that have the <a href="https://msdn.microsoft.com/en-us/library/Bb774732(v=VS.85).aspx">LVS_EX_CHECKBOXES</a> style. 


## -parameters




### -param hwndLV

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to a list-view control. 


### -param i

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The index of the item for which to retrieve the check state. 

