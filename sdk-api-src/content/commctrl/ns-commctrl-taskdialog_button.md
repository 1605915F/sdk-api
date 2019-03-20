---
UID: NS:commctrl._TASKDIALOG_BUTTON
title: TASKDIALOG_BUTTON (commctrl.h)
author: windows-sdk-content
description: The TASKDIALOG_BUTTON structure contains information used to display a button in a task dialog. The TASKDIALOGCONFIG structure uses this structure.
old-location: controls\TASKDIALOG_BUTTON.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\taskdialogs\taskdialogreference\taskdialogstructures\taskdialog_button.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TASKDIALOG_BUTTON, TASKDIALOG_BUTTON structure [Windows Controls], _shell_TASKDIALOG_BUTTON, _shell_TASKDIALOG_BUTTON_cpp, commctrl/TASKDIALOG_BUTTON, controls.TASKDIALOG_BUTTON, controls._shell_TASKDIALOG_BUTTON
ms.topic: struct
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - TASKDIALOG_BUTTON
product: Windows
targetos: Windows
req.typenames: TASKDIALOG_BUTTON
req.redist: 
---

# TASKDIALOG_BUTTON structure


## -description


The <b>TASKDIALOG_BUTTON</b> structure contains information used to display a button in a task dialog. The <a href="https://msdn.microsoft.com/en-us/library/Bb787473(v=VS.85).aspx">TASKDIALOGCONFIG</a> structure uses this structure.


## -struct-fields




### -field nButtonID

Type: <b>int</b>

Indicates the value to be returned when this button is selected.


### -field pszButtonText

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">PCWSTR</a></b>

Pointer that references the string to be used to label the button. This parameter can be either a null-terminated string or an integer resource identifier passed to the <a href="https://msdn.microsoft.com/en-us/library/ms648029(v=VS.85).aspx">MAKEINTRESOURCE</a> macro. When using Command Links, you delineate the command from the note by placing a new line character in the string.

