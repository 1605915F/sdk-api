---
UID: NF:tom.ITextDocument.Undo
title: ITextDocument::Undo (tom.h)
author: windows-sdk-content
description: Performs a specified number of undo operations.
old-location: controls\ITextDocument_Undo.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\undo.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITextDocument interface [Windows Controls],Undo method, ITextDocument.Undo, ITextDocument::Undo, Undo, Undo method [Windows Controls], Undo method [Windows Controls],ITextDocument interface, _win32_ITextDocument_Undo, _win32_ITextDocument_Undo_cpp, controls.ITextDocument_Undo, controls._win32_ITextDocument_Undo, tom/ITextDocument::Undo
ms.topic: method
req.header: tom.h
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
req.dll: Msftedit.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Msftedit.dll
api_name:
 - ITextDocument.Undo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITextDocument::Undo


## -description


Performs a specified number of undo operations.


## -parameters




### -param Count

Type: <b>long</b>

The specified number of undo operations. If the value of this parameter is <b>tomFalse</b>, undo processing is suspended. If this parameter is <b>tomTrue</b>, undo processing is restored. 


### -param pCount

Type: <b>long*</b>

The actual count of undo operations performed. This parameter can be <b>NULL</b>. 


## -returns



Type: <b>HRESULT</b>

If all of the 
						<i>Count</i> undo operations were performed, it returns <b>S_OK</b>. If the method fails, it returns <b>S_FALSE</b>, indicating that less than 
						<i>Count</i> undo operations were performed. For more information on COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb774052(v=VS.85).aspx">ITextDocument</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb774101(v=VS.85).aspx">Redo</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

