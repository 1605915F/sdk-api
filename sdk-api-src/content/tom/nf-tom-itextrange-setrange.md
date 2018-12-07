---
UID: NF:tom.ITextRange.SetRange
title: ITextRange::SetRange
author: windows-sdk-content
description: Adjusts the range endpoints to the specified values.
old-location: controls\ITextRange_SetRange.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\setrange.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextRange interface [Windows Controls],SetRange method, ITextRange.SetRange, ITextRange::SetRange, SetRange, SetRange method [Windows Controls], SetRange method [Windows Controls],ITextRange interface, _win32_ITextRange_SetRange, _win32_ITextRange_SetRange_cpp, controls.ITextRange_SetRange, controls._win32_ITextRange_SetRange, tom/ITextRange::SetRange
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ITextRange.SetRange
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextRange::SetRange


## -description


Adjusts the range endpoints to the specified values. 


## -parameters




### -param cpAnchor

Type: <b>long</b>

The character position for the anchor end of the range. 


### -param cpActive

Type: <b>long</b>

The character position for the active end of the range. 


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This method sets the range's start position to <code>min(cpActive, cpAnchor)</code>, and the end position to <code>max(cpActive, cpAnchor)</code>. If the range is a nondegenerate selection, <i>cpAnchor</i> is the active end, and <i>cpAnchor</i> is the anchor end.  If the range is a degenerate selection, the selection is displayed at the start of the line, rather than at the end of the previous line.

This method removes any other subranges this range may have. To preserve the current subranges, use <a href="https://msdn.microsoft.com/a635edd3-dcb9-4f1f-bf6e-774ce3f0c505">ITextRange2::SetActiveSubrange</a>. 


If the text range is a selection, you can set the attributes of the selection by using the <a href="https://msdn.microsoft.com/en-us/library/Bb774143(v=VS.85).aspx">ITextSelection::SetFlags</a> method. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb774058(v=VS.85).aspx">ITextRange</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

