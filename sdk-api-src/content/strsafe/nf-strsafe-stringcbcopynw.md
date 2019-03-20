---
UID: NF:strsafe.StringCbCopyNW
title: StringCbCopyNW function (strsafe.h)
author: windows-sdk-content
description: Copies the specified number of bytes from one string to another.
old-location: menurc\stringcbcopyn.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\strings\stringreference\stringfunctions\stringcbcopyn.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: StringCbCopyN, StringCbCopyN function [Menus and Other Resources], StringCbCopyNA, StringCbCopyNW, _shell_StringCbCopyN, _shell_stringcbcopyn_cpp, menurc.stringcbcopyn, strsafe/StringCbCopyN, strsafe/StringCbCopyNA, strsafe/StringCbCopyNW, winui._shell_stringcbcopyn
ms.topic: function
req.header: strsafe.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: StringCbCopyNW (Unicode) and StringCbCopyNA (ANSI)
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
 - Strsafe.h
api_name:
 - StringCbCopyN
 - StringCbCopyNA
 - StringCbCopyNW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# StringCbCopyNW function


## -description


Copies the specified number of bytes from one string to another. The size of the destination buffer is provided to the function to ensure that it does not write past the end of this buffer.

<b>StringCbCopyN</b> is a replacement for the following functions:
<ul>
<li><a href="http://go.microsoft.com/fwlink/p/?linkid=192506">strncpy, wcsncpy, _tcsncpy</a></li>
</ul>

## -parameters




### -param pszDest [out]

Type: <b>LPTSTR</b>

The destination buffer, which receives the copied characters.


### -param cbDest [in]

Type: <b>size_t</b>

The size of <i>pszDest</i>, in bytes. This value must be large enough to hold the copied bytes (the size of <i>pszSrc</i> or the value of <i>cbSrc</i>, whichever is smaller) and also account for the terminating null character. The maximum number of characters allowed is <code>STRSAFE_MAX_CCH * sizeof(TCHAR)</code>.


### -param pszSrc [in]

Type: <b>LPCTSTR</b>

The source string. This string must be null-terminated.


### -param cbToCopy [in]

Type: <b>size_t</b>

The maximum number of bytes to be copied from <i>pszSrc</i> to <i>pszDest</i>.


## -returns



Type: <b>HRESULT</b>

This function can return one of the following values. It is strongly recommended that you use the <a href="https://msdn.microsoft.com/7a258b0b-d214-46c5-be0a-6493cd14a0e5">SUCCEEDED</a> and <a href="https://msdn.microsoft.com/d9c4ff73-c255-4a82-b901-23bd5b41ee6c">FAILED</a> macros to test the return value of this function.

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
Source data was present, the data was copied from <i>pszSrc</i> without truncation, and the resultant destination buffer is null-terminated.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STRSAFE_E_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The value in <i>cbDest</i> is either larger than <code>STRSAFE_MAX_CCH * sizeof(TCHAR)</code>, or the destination buffer is already full.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STRSAFE_E_INSUFFICIENT_BUFFER</b></dt>
</dl>
</td>
<td width="60%">
The copy operation failed due to insufficient buffer space. The destination buffer contains a truncated, null-terminated version of the intended result. In situations where truncation is acceptable, this may not necessarily be seen as a failure condition.

</td>
</tr>
</table>
 

Note that this function returns an <b>HRESULT</b> value, unlike the functions that it replaces.




## -remarks



<b>StringCbCopyN</b> provides additional processing for proper buffer handling in your code. Poor buffer handling is implicated in many security issues that involve buffer overruns. <b>StringCbCopyN</b> always null-terminates and never overflows a valid destination buffer, even if the contents of the source string change during the operation.

While this routine is meant as a replacement for <a href="https://msdn.microsoft.com/library/xdsywd25(v=VS.100).aspx">strncpy</a>, there are differences in behavior. If <i>cbSrc</i> is larger than the number of bytes in <i>pszSrc</i>, <b>StringCbCopyN</b>—unlike <b>strncpy</b>—does not continue to pad <i>pszDest</i> with null characters until <i>cbSrc</i> bytes have been copied.

Behavior is undefined if the strings pointed to by <i>pszSrc</i> and <i>pszDest</i> overlap.

Neither <i>pszSrc</i> nor <i>pszDest</i> should be <b>NULL</b>. See <a href="https://msdn.microsoft.com/en-us/library/ms647503(v=VS.85).aspx">StringCbCopyNEx</a> if you require the handling of null string pointer values.

<b>StringCbCopyN</b> can be used in its generic form, or in its more specific forms. The data type of the string determines the form of this function that you should use, as shown in the following table.

<table class="clsStd">
<tr>
<th>String Data Type</th>
<th>String Literal</th>
<th>Function</th>
</tr>
<tr>
<td><b>char</b></td>
<td>"string"</td>
<td><b>StringCbCopyNA</b></td>
</tr>
<tr>
<td><b>TCHAR</b></td>
<td>TEXT("string")</td>
<td><b>StringCbCopyN</b></td>
</tr>
<tr>
<td><b>WCHAR</b></td>
<td>L"string"</td>
<td><b>StringCbCopyNW</b></td>
</tr>
</table>
 




## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms647499(v=VS.85).aspx">StringCbCopy</a>



<a href="https://msdn.microsoft.com/en-us/library/ms647503(v=VS.85).aspx">StringCbCopyNEx</a>



<a href="https://msdn.microsoft.com/en-us/library/ms647530(v=VS.85).aspx">StringCchCopyN</a>
 

 

