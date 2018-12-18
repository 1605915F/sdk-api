---
UID: NF:propvarutil.InitVariantFromInt64Array
title: InitVariantFromInt64Array function
author: windows-sdk-content
description: Initializes a VARIANT structure with an array of 64-bit integer values.
old-location: properties\InitVariantFromInt64Array.htm
tech.root: properties
ms.assetid: 18e9c804-b5e4-4abe-adcd-eaa402c6c94a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitVariantFromInt64Array, InitVariantFromInt64Array function [Windows Properties], _shell_InitVariantFromInt64Array, properties.InitVariantFromInt64Array, propvarutil/InitVariantFromInt64Array, shell.InitVariantFromInt64Array
ms.topic: function
req.header: propvarutil.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Propsys.lib
req.dll: Propsys.dll (version 6.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Propsys.dll
api_name:
 - InitVariantFromInt64Array
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitVariantFromInt64Array function


## -description


Initializes a <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure with an array of 64-bit integer values.


## -parameters




### -param prgn [in]

Type: <b>const LONGLONG*</b>

Pointer to the source array of <b>LONGLONG</b> values.


### -param cElems [in]

Type: <b>ULONG</b>

The number of elements in the array pointed to by <i>prgn</i>.

The number of array elements.


### -param pvar [out]

Type: <b>VARIANT*</b>

When this function returns, contains the initialized <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_ARRAY | VT_I8 variant.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="shell.InitVariantFromInt64Array">InitVariantFromInt64Array</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>LONGLONG rgLongs[] = {4, 2};
VARIANT var;

HRESULT hr = InitVariantFromInt64Array(rgLongs, ARRAYSIZE(rgLongs), &amp;var);

if (SUCCEEDED(hr))                            
{
    // var now is valid and has type VT_ARRAY | VT_I8.
    VariantClear(&amp;propvar);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="shell.InitPropVariantFromInt64Vector">InitPropVariantFromInt64Vector</a>



<a href="shell.InitVariantFromInt64">InitVariantFromInt64</a>



<a href="shell.VariantToInt64Array">VariantToInt64Array</a>
 

 

