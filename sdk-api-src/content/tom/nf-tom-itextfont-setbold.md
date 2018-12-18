---
UID: NF:tom.ITextFont.SetBold
title: ITextFont::SetBold
author: windows-sdk-content
description: Sets whether characters are bold.
old-location: controls\ITextFont_SetBold.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\setbold.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextFont interface [Windows Controls],SetBold method, ITextFont.SetBold, ITextFont::SetBold, SetBold, SetBold method [Windows Controls], SetBold method [Windows Controls],ITextFont interface, _win32_ITextFont_SetBold, _win32_ITextFont_SetBold_cpp, controls.ITextFont_SetBold, controls._win32_ITextFont_SetBold, tom/ITextFont::SetBold
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
 - ITextFont.SetBold
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextFont::SetBold


## -description


Sets whether characters are bold.


## -parameters




### -param Value [in]

Type: <b>long</b>

A <a href="https://msdn.microsoft.com/en-us/library/Bb787724(v=VS.85).aspx">tomBool</a> value that can be one of the following.

<table class="clsStd">
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td><b>tomTrue</b></td>
<td>Characters are bold.</td>
</tr>
<tr>
<td><b>tomFalse</b></td>
<td>Characters are not bold.</td>
</tr>
<tr>
<td><b>tomToggle</b></td>
<td>Toggle the state of the Bold property.</td>
</tr>
<tr>
<td><b>tomUndefined</b></td>
<td>The Bold property is undefined.</td>
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
Invalid argument

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
<tr>
<td width="40%">
<dl>
<dt><b>E_ACCESSDENIED</b></dt>
</dl>
</td>
<td width="60%">
Write access is denied.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory.

</td>
</tr>
</table>
 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb773935(v=VS.85).aspx">GetBold</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb774040(v=VS.85).aspx">GetWeight</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb774054(v=VS.85).aspx">ITextFont</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787833(v=VS.85).aspx">SetWeight</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

