---
UID: NF:windowsx.ComboBox_ShowDropdown
title: ComboBox_ShowDropdown macro
author: windows-sdk-content
description: Shows or hides the list in a combo box. You can use this macro or send the CB_SHOWDROPDOWN message explicitly.
old-location: controls\ComboBox_ShowDropdown.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\comboboxes\comboboxreference\comboboxmacros\combobox_showdropdown.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ComboBox_ShowDropdown, ComboBox_ShowDropdown macro [Windows Controls], _win32_ComboBox_ShowDropdown, _win32_ComboBox_ShowDropdown_cpp, controls.ComboBox_ShowDropdown, controls._win32_ComboBox_ShowDropdown, windowsx/ComboBox_ShowDropdown
ms.topic: macro
req.header: windowsx.h
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
 - Windowsx.h
api_name:
 - ComboBox_ShowDropdown
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ComboBox_ShowDropdown macro


## -description


Shows or hides the list in a combo box. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb775919(v=VS.85).aspx">CB_SHOWDROPDOWN</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param fShow

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

<b>TRUE</b> to show the dropdown, or <b>FALSE</b> to hide it.


## -remarks



This macro has no effect on a combo box created with the <a href="https://msdn.microsoft.com/en-us/library/Bb775796(v=VS.85).aspx">CBS_SIMPLE</a> style.
	



