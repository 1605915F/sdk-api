---
UID: NF:winuser.SetDlgItemInt
title: SetDlgItemInt function (winuser.h)
author: windows-sdk-content
description: Sets the text of a control in a dialog box to the string representation of a specified integer value.
old-location: dlgbox\setdlgitemint.htm
tech.root: dlgbox
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\dialogboxes\dialogboxreference\dialogboxfunctions\setdlgitemint.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetDlgItemInt, SetDlgItemInt function [Dialog Boxes], _win32_SetDlgItemInt, _win32_setdlgitemint_cpp, dlgbox.setdlgitemint, winui._win32_setdlgitemint, winuser/SetDlgItemInt
ms.topic: function
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
 - ext-ms-win-ntuser-dialogbox-l1-1-2.dll
api_name:
 - SetDlgItemInt
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetDlgItemInt function


## -description


Sets the text of a control in a dialog box to the string representation of a specified integer value. 


## -parameters




### -param hDlg [in]

Type: <b>HWND</b>

A handle to the dialog box that contains the control. 


### -param nIDDlgItem [in]

Type: <b>int</b>

The control to be changed. 


### -param uValue [in]

Type: <b>UINT</b>

The integer value used to generate the item text. 


### -param bSigned [in]

Type: <b>BOOL</b>

Indicates whether the <i>uValue</i> parameter is signed or unsigned. If this parameter is <b>TRUE</b>, <i>uValue</i> is signed. If this parameter is <b>TRUE</b> and <i>uValue</i> is less than zero, a minus sign is placed before the first digit in the string. If this parameter is <b>FALSE</b>, <i>uValue</i> is unsigned. 


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. 




## -remarks



To set the new text, this function sends a <a href="https://msdn.microsoft.com/en-us/library/ms632644(v=VS.85).aspx">WM_SETTEXT</a> message to the specified control.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632588(v=VS.85).aspx">Dialog Boxes</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645485(v=VS.85).aspx">GetDlgItemInt</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms645521(v=VS.85).aspx">SetDlgItemText</a>



<a href="https://msdn.microsoft.com/en-us/library/ms632644(v=VS.85).aspx">WM_SETTEXT</a>
 

 

