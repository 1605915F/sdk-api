---
UID: NF:winuser.IsDlgButtonChecked
title: IsDlgButtonChecked function
author: windows-sdk-content
description: The IsDlgButtonChecked function determines whether a button control is checked or whether a three-state button control is checked, unchecked, or indeterminate.
old-location: controls\IsDlgButtonChecked.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\buttons\buttonreference\buttonfunctions\isdlgbuttonchecked.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IsDlgButtonChecked, IsDlgButtonChecked function [Windows Controls], _win32_IsDlgButtonChecked, _win32_IsDlgButtonChecked_cpp, controls.IsDlgButtonChecked, controls._win32_IsDlgButtonChecked, winuser/IsDlgButtonChecked
ms.topic: function
req.header: winuser.h
req.include-header: Windows.h
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
 - Ext-MS-Win-NTUser-DialogBox-l1-1-0.dll
 - Ext-MS-Win-NTUser-DialogBox-l1-1-1.dll
 - ext-ms-win-ntuser-dialogbox-l1-1-2.dll
api_name:
 - IsDlgButtonChecked
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IsDlgButtonChecked function


## -description


The <b>IsDlgButtonChecked</b> function determines whether a button control is checked or whether a three-state button control is checked, unchecked, or indeterminate. 


## -parameters




### -param hDlg [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the dialog box that contains the button control. 


### -param nIDButton [in]

Type: <b>int</b>

The identifier of the button control. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The return value from a button created with the <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_AUTOCHECKBOX</a>, <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_AUTORADIOBUTTON</a>, <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_AUTO3STATE</a>, <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_CHECKBOX</a>, <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_RADIOBUTTON</a>, or <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_3STATE</a> styles can be one of the values in the following table. If the button has any other style, the return value is zero. 
				

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>BST_CHECKED</b></dt>
</dl>
</td>
<td width="60%">
The button is checked.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>BST_INDETERMINATE</b></dt>
</dl>
</td>
<td width="60%">
The button is in an indeterminate state (applies only if the button has the <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_3STATE</a> or <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_AUTO3STATE</a> style).

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>BST_UNCHECKED</b></dt>
</dl>
</td>
<td width="60%">
The button is not checked.

</td>
</tr>
</table>
 




## -remarks



The <b>IsDlgButtonChecked</b> function sends a <a href="https://msdn.microsoft.com/en-us/library/Bb775986(v=VS.85).aspx">BM_GETCHECK</a> message to the specified button control. 


#### Examples

For an example, see the section titled "Creating a Modeless Dialog Box" in <a href="https://msdn.microsoft.com/en-us/library/ms644996(v=VS.85).aspx">Using Dialog Boxes</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb761875(v=VS.85).aspx">CheckDlgButton</a>
 

 

