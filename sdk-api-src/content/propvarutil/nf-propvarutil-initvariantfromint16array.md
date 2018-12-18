---
UID: NF:propvarutil.InitVariantFromInt16Array
title: InitVariantFromInt16Array function
author: windows-sdk-content
description: Initializes a VARIANT structure with an array of 16-bit integer values.
old-location: properties\InitVariantFromInt16Array.htm
tech.root: properties
ms.assetid: 6aeca46e-96b5-42cb-b5db-2c1e3152d629
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitVariantFromInt16Array, InitVariantFromInt16Array function [Windows Properties], _shell_InitVariantFromInt16Array, properties.InitVariantFromInt16Array, propvarutil/InitVariantFromInt16Array, shell.InitVariantFromInt16Array
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
 - InitVariantFromInt16Array
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitVariantFromInt16Array function


## -description


Initializes a <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure with an array of 16-bit integer values.


## -parameters




### -param prgn [in]

Type: <b>const SHORT*</b>

Pointer to the source array of <b>SHORT</b> values.


### -param cElems [in]

Type: <b>ULONG</b>

The number of elements in the array pointed to by <i>prgn</i>.


### -param pvar [out]

Type: <b>VARIANT*</b>

When this function returns, contains the initialized <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_ARRAY | VT_I2 variant.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="shell.InitVariantFromInt16Array">InitVariantFromInt16Array</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>SHORT rgShorts[] = {3, 1};
VARIANT var;

HRESULT hr = InitVariantFromInt16Array(rgShorts, ARRAYSIZE(rgShorts), &amp;var);

if (SUCCEEDED(hr))
{
    // var now is valid and has type VT_ARRAY | VT_I2.
    VariantClear(&amp;propvar);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="shell.InitPropVariantFromInt16Vector">InitPropVariantFromInt16Vector</a>



<a href="shell.InitVariantFromInt16">InitVariantFromInt16</a>



<a href="shell.VariantToInt16Array">VariantToInt16Array</a>
 

 

