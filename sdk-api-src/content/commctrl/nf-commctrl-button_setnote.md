---
UID: NF:commctrl.Button_SetNote
title: Button_SetNote macro (commctrl.h)
author: windows-sdk-content
description: Sets the text of the note associated with a specified command link button. You can use this macro or send the BCM_SETNOTE message explicitly.
old-location: controls\Button_SetNote.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\buttons\buttonreference\buttonmacros\button_setnote.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Button_SetNote, Button_SetNote macro [Windows Controls], _shell_Button_SetNote, _shell_Button_SetNote_cpp, commctrl/Button_SetNote, controls.Button_SetNote, controls._shell_Button_SetNote
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
 - Button_SetNote
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# Button_SetNote macro


## -description


Sets the text of the note associated with a specified command link button. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb775977(v=VS.85).aspx">BCM_SETNOTE</a> message explicitly.


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the button control. 


### -param psz

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">PCWSTR</a></b>

A pointer to a null-terminated <b>WCHAR</b> string that contains the note.


## -remarks



Beginning with comctl32 DLL version 6.01, command link buttons may have a note.

This macro works only with the <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_COMMANDLINK</a> and <a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">BS_DEFCOMMANDLINK</a> button styles.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb775951(v=VS.85).aspx">Button Styles</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb775947(v=VS.85).aspx">Button Types</a>



<b>Conceptual</b>



<b>Reference</b>
 

 

