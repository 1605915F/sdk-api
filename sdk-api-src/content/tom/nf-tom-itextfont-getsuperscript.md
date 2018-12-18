---
UID: NF:tom.ITextFont.GetSuperscript
title: ITextFont::GetSuperscript
author: windows-sdk-content
description: Gets whether characters are displayed as superscript.
old-location: controls\ITextFont_GetSuperscript.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\getsuperscript.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetSuperscript, GetSuperscript method [Windows Controls], GetSuperscript method [Windows Controls],ITextFont interface, ITextFont interface [Windows Controls],GetSuperscript method, ITextFont.GetSuperscript, ITextFont::GetSuperscript, _win32_ITextFont_GetSuperscript, _win32_ITextFont_GetSuperscript_cpp, controls.ITextFont_GetSuperscript, controls._win32_ITextFont_GetSuperscript, tom/ITextFont::GetSuperscript
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
 - ITextFont.GetSuperscript
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextFont::GetSuperscript


## -description


Gets whether characters are displayed as superscript.


## -parameters




### -param pValue

Type: <b>long*</b>

A <a href="https://msdn.microsoft.com/en-us/library/Bb787724(v=VS.85).aspx">tomBool</a> value that can be one of the following.

<table class="clsStd">
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td><b>tomTrue</b></td>
<td>Characters are displayed as superscript.</td>
</tr>
<tr>
<td><b>tomFalse</b></td>
<td>Characters are not displayed as superscript.</td>
</tr>
<tr>
<td><b>tomUndefined</b></td>
<td>The Superscript property is undefined.</td>
</tr>
</table>
 


## -returns



Type: <b>HRESULT</b>

If the method succeeds, it returns <b>S_OK</b>. If the method fails, it returns one of the following COM error codes. For more information about COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.

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
<tr>
<td width="40%">
<dl>
<dt><b>CO_E_RELEASED</b></dt>
</dl>
</td>
<td width="60%">
The font object is attached to a range that has been deleted.

</td>
</tr>
</table>
 




## -remarks



This property corresponds to the <b>CFE_SUPERSCRIPT</b> effect described in the <a href="https://msdn.microsoft.com/en-us/library/Bb787883(v=VS.85).aspx">CHARFORMAT2</a> structure.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb787883(v=VS.85).aspx">CHARFORMAT2</a>



<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb774054(v=VS.85).aspx">ITextFont</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787830(v=VS.85).aspx">SetSuperscript</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

