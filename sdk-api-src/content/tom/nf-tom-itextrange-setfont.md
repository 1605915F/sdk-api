---
UID: NF:tom.ITextRange.SetFont
title: ITextRange::SetFont (tom.h)
author: windows-sdk-content
description: Sets this range's character attributes to those of the specified ITextFont object.
old-location: controls\ITextRange_SetFont.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\setfont.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITextRange interface [Windows Controls],SetFont method, ITextRange.SetFont, ITextRange::SetFont, SetFont, SetFont method [Windows Controls], SetFont method [Windows Controls],ITextRange interface, _win32_ITextRange_SetFont, _win32_ITextRange_SetFont_cpp, controls.ITextRange_SetFont, controls._win32_ITextRange_SetFont, tom/ITextRange::SetFont
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
 - ITextRange.SetFont
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextRange::SetFont


## -description


Sets this range's character attributes to those of the specified <a href="https://msdn.microsoft.com/en-us/library/Bb774054(v=VS.85).aspx">ITextFont</a> object.


## -parameters




### -param pFont [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb774054(v=VS.85).aspx">ITextFont</a>*</b>

A font object with the desired character format. 


## -returns



Type: <b>HRESULT</b>

The method returns an <b>HRESULT</b> value. If the method succeeds, it returns <b>S_OK</b>. If the method fails, it returns one of the following error codes. For more information about COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Value</b></dt>
</dl>
</td>
<td width="60%">
Meaning

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_ACCESSDENIED</b></dt>
</dl>
</td>
<td width="60%">
Text is protected.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
<i>pFont</i> is null.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Out of memory.

</td>
</tr>
</table>
 




## -remarks



For occasional format changes, use the <b>ITextRange::SetFont</b> method. However, to make a number of character formatting changes, it is more efficient to use a font duplicate. This is because every time you execute a statement like <code>range.font.bold = tomTrue</code>, a font object is allocated and freed. However, a font duplicate can be allocated once and used many times. Furthermore, you can save the font duplicate, reset it to the default or undefined states with the <a href="https://msdn.microsoft.com/en-us/library/Bb787865(v=VS.85).aspx">Reset</a> method, and give it values as needed for your rich-text processing. For sample code that shows how to use font duplicates, see <a href="https://msdn.microsoft.com/en-us/library/Bb787726(v=VS.85).aspx">Using a Font Duplicate</a>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb774058(v=VS.85).aspx">ITextRange</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787865(v=VS.85).aspx">Reset</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

