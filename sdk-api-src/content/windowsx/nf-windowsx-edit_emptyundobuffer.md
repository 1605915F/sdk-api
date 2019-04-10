---
UID: NF:windowsx.Edit_EmptyUndoBuffer
title: Edit_EmptyUndoBuffer macro (windowsx.h)
author: windows-sdk-content
description: Resets the undo flag of an edit or rich edit control. The undo flag is set whenever an operation within the edit control can be undone. You can use this macro or send the EM_EMPTYUNDOBUFFER message explicitly.
old-location: controls\Edit_EmptyUndoBuffer.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\editcontrols\editcontrolreference\editcontrolmacros\edit_emptyundobuffer.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Edit_EmptyUndoBuffer, Edit_EmptyUndoBuffer macro [Windows Controls], _win32_Edit_EmptyUndoBuffer, _win32_Edit_EmptyUndoBuffer_cpp, controls.Edit_EmptyUndoBuffer, controls._win32_Edit_EmptyUndoBuffer, windowsx/Edit_EmptyUndoBuffer
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
 - Edit_EmptyUndoBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# Edit_EmptyUndoBuffer macro


## -description


Resets the undo flag of an edit or rich edit control. The undo flag is set whenever an operation within the edit control can be undone. You can use this macro or send the <a href="https://msdn.microsoft.com/en-us/library/Bb761568(v=VS.85).aspx">EM_EMPTYUNDOBUFFER</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


## -remarks



For more information, see <a href="https://msdn.microsoft.com/en-us/library/Bb761568(v=VS.85).aspx">EM_EMPTYUNDOBUFFER</a>.



