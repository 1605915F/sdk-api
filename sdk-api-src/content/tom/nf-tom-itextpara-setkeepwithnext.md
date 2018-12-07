---
UID: NF:tom.ITextPara.SetKeepWithNext
title: ITextPara::SetKeepWithNext
author: windows-sdk-content
description: Controls whether page breaks are allowed between the paragraphs in a range.
old-location: controls\ITextPara_SetKeepWithNext.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\richedit\textobjectmodel\textobjectmodelreference\textobjectmodelinterfaces\setkeepwithnext.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITextPara interface [Windows Controls],SetKeepWithNext method, ITextPara.SetKeepWithNext, ITextPara::SetKeepWithNext, SetKeepWithNext, SetKeepWithNext method [Windows Controls], SetKeepWithNext method [Windows Controls],ITextPara interface, _win32_ITextPara_SetKeepWithNext, _win32_ITextPara_SetKeepWithNext_cpp, controls.ITextPara_SetKeepWithNext, controls._win32_ITextPara_SetKeepWithNext, tom/ITextPara::SetKeepWithNext
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
 - ITextPara.SetKeepWithNext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITextPara::SetKeepWithNext


## -description


Controls whether page breaks are allowed between the paragraphs in a range.


## -parameters




### -param Value [in]

Type: <b>long</b>

Indicates if page breaks can be used between the paragraphs of a range. It can be one of the following possible values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
<dt>tomTrue</dt>
</dl>
</td>
<td width="60%">
Page breaks are not allowed between paragraphs.

</td>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
<dt>tomFalse</dt>
</dl>
</td>
<td width="60%">
Page breaks are allowed between paragraphs.

</td>
</tr>
<tr>
<td width="40%"><a id=""></a><dl>
<dt><b></b></dt>
<dt>tomUndefined</dt>
</dl>
</td>
<td width="60%">
The property is undefined.

</td>
</tr>
</table>
 


## -returns



Type: <b>HRESULT</b>

If <b>ITextPara::SetKeepWithNext</b> succeeds, it returns <b>S_OK</b>. If the method fails, it returns one of the following COM error codes. For more information about COM error codes, see <a href="https://msdn.microsoft.com/15f3ae3e-1794-4948-a7aa-6309a703364b">Error Handling in COM</a>.

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
<tr>
<td width="40%">
<dl>
<dt><b>CO_E_RELEASED</b></dt>
</dl>
</td>
<td width="60%">
The paragraph formatting object is attached to a range that has been deleted.

</td>
</tr>
</table>
 




## -remarks



This property corresponds to the PFE_KEEPNEXT effect described in the <a href="https://msdn.microsoft.com/en-us/library/Bb787942(v=VS.85).aspx">PARAFORMAT2</a> structure. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb774056(v=VS.85).aspx">ITextPara</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb787942(v=VS.85).aspx">PARAFORMAT2</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb787607(v=VS.85).aspx">Text Object Model</a>
 

 

