---
UID: NF:tom.ITextDocument.GetSaved
title: ITextDocument::GetSaved
author: windows-sdk-content
description: Gets a value that indicates whether changes have been made since the file was last saved.
old-location: controls\ITextDocument_GetSaved.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\getsaved.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetSaved, GetSaved method [Windows Controls], GetSaved method [Windows Controls],ITextDocument interface, ITextDocument interface [Windows Controls],GetSaved method, ITextDocument.GetSaved, ITextDocument::GetSaved, _win32_ITextDocument_GetSaved, _win32_ITextDocument_GetSaved_cpp, controls.ITextDocument_GetSaved, controls._win32_ITextDocument_GetSaved, tom/ITextDocument::GetSaved
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
 - ITextDocument.GetSaved
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextDocument::GetSaved


## -description


Gets a value that indicates whether changes have been made since the file was last saved. 


## -parameters




### -param pValue

Type: <b>long*</b>

The value <b>tomTrue</b> if no changes have been made since the file was last saved, or the value <b>tomFalse</b> if there are unsaved changes.


## -returns



Type: <b>HRESULT</b>

If the method succeeds, it returns <b>S_OK</b>. If the method fails, it returns the following COM error code. For more information about COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument.

</td>
</tr>
</table>
 




## -remarks



To set the saved property, call the <a href="https://msdn.microsoft.com/en-us/library/Bb787809(v=VS.85).aspx">ITextDocument::SetSaved</a> method.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb774052(v=VS.85).aspx">ITextDocument</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787809(v=VS.85).aspx">SetSaved</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

