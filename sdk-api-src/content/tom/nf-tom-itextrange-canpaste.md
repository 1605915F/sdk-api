---
UID: NF:tom.ITextRange.CanPaste
title: ITextRange::CanPaste
author: windows-sdk-content
description: Determines if a data object can be pasted, using a specified format, into the current range.
old-location: controls\ITextRange_CanPaste.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\canpaste.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CanPaste, CanPaste method [Windows Controls], CanPaste method [Windows Controls],ITextRange interface, ITextRange interface [Windows Controls],CanPaste method, ITextRange.CanPaste, ITextRange::CanPaste, _win32_ITextRange_CanPaste, _win32_ITextRange_CanPaste_cpp, controls.ITextRange_CanPaste, controls._win32_ITextRange_CanPaste, tom/ITextRange::CanPaste
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
 - ITextRange.CanPaste
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextRange::CanPaste


## -description


Determines if a data object can be pasted, using a specified format, into the current range. 


## -parameters




### -param pVar

Type: <b>VARIANT*</b>

The 
					<a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a> to be pasted. However, the Clipboard contents are checked for pasting if any of the following are true: 
					

<ul>
<li><i>pVar</i> is null </li>
<li><i>pVar</i>-&gt;punkVal is null </li>
<li><i>pVar</i>-&gt;vt is not <b>VT_UNKNOWN</b></li>
<li><i>pVar</i>-&gt;punkVal does not return an 
							<a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a> object when queried for one </li>
</ul>

### -param Format

Type: <b>long</b>

Clipboard format that is used. Zero represents the best format, which usually is RTF, but <b>CF_UNICODETEXT</b> and other formats are also possible. The default value is zero. 


### -param pValue

Type: <b>long*</b>

A <a href="https://msdn.microsoft.com/en-us/library/Bb787724(v=VS.85).aspx">tomBool</a> value that is <b>tomTrue</b> only if the data object identified by 
					<i>pVar</i> can be pasted, using the specified format, into the range. This parameter can null. 


## -returns



Type: <b>HRESULT</b>

The method returns the following COM error codes. For more information on COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The clipboard contents or <a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a> can be pasted.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The clipboard contents or <a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a> cannot be pasted.

</td>
</tr>
</table>
 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787742(v=VS.85).aspx">Copy</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb774058(v=VS.85).aspx">ITextRange</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

