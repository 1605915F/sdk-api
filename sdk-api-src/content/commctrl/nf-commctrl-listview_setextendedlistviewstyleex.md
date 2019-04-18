---
UID: NF:commctrl.ListView_SetExtendedListViewStyleEx
title: ListView_SetExtendedListViewStyleEx macro (commctrl.h)
author: windows-sdk-content
description: Sets extended styles for list-view controls using the style mask. You can use this macro or send the LVM_SETEXTENDEDLISTVIEWSTYLE message explicitly.
old-location: controls\ListView_SetExtendedListViewStyleEx.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\listview\macros\listview_setextendedlistviewstyleex.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ListView_SetExtendedListViewStyleEx, ListView_SetExtendedListViewStyleEx macro [Windows Controls], _win32_ListView_SetExtendedListViewStyleEx, _win32_ListView_SetExtendedListViewStyleEx_cpp, commctrl/ListView_SetExtendedListViewStyleEx, controls.ListView_SetExtendedListViewStyleEx, controls._win32_ListView_SetExtendedListViewStyleEx
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
 - ListView_SetExtendedListViewStyleEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ListView_SetExtendedListViewStyleEx macro


## -description


Sets extended styles for list-view controls using the style mask. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761165(v=VS.85).aspx">LVM_SETEXTENDEDLISTVIEWSTYLE</a> message explicitly.


## -parameters




### -param hwndLV

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the list-view control that will receive the style change. 


### -param dwMask

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

A <b>DWORD</b> value that specifies which styles in 
					<i>dwExStyle</i> are to be affected. This parameter can be a combination of <a href="https://msdn.microsoft.com/en-us/library/Bb774732(v=VS.85).aspx">Extended List-View Styles</a>. Only the extended styles in <i>dwExMask</i> will be changed. All other styles will be maintained as they are. If this parameter is zero, all of the styles in <i>dwExStyle</i> will be affected. 


### -param dw

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

A <b>DWORD</b> value that specifies the extended list-view control styles to set. This parameter can be a combination of <a href="https://msdn.microsoft.com/en-us/library/Bb774732(v=VS.85).aspx">Extended List-View Styles</a>. Styles that are not set, but that are specified in <i>dwExMask</i>, are removed.


## -remarks



When you use this macro to set the <a href="https://msdn.microsoft.com/en-us/library/Bb774732(v=VS.85).aspx">LVS_EX_CHECKBOXES</a> style, any previously set state image index will be discarded. All check boxes will be initialized to the unchecked state. The state image index is contained in bits 12 through 15 of the 
<b>state</b> member of the <a href="https://msdn.microsoft.com/en-us/library/Bb774760(v=VS.85).aspx">LVITEM</a> structure.



