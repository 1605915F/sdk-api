---
UID: NF:propvarutil.VariantToDoubleArray
title: VariantToDoubleArray function
author: windows-sdk-content
description: Extracts an array of DOUBLE values from a VARIANT structure.
old-location: properties\VariantToDoubleArray.htm
tech.root: properties
ms.assetid: 6830c2e2-d19a-45d5-af15-debfb08548bc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: VariantToDoubleArray, VariantToDoubleArray function [Windows Properties], _shell_VariantToDoubleArray, properties.VariantToDoubleArray, propvarutil/VariantToDoubleArray, shell.VariantToDoubleArray
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
 - VariantToDoubleArray
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# VariantToDoubleArray function


## -description


Extracts an array of <b>DOUBLE</b> values from a <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


## -parameters




### -param var [in]

Type: <b>REFVARIANT</b>

Reference to a source <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


### -param prgn [out]

Type: <b>DOUBLE*</b>

Pointer to a buffer that contains <i>crgn</i> <b>DOUBLE</b> values. When this function returns, the buffer has been initialized with *<i>pcElem</i> <b>DOUBLE</b> elements extracted from the source <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


### -param crgn [in]

Type: <b>ULONG</b>

The number of elements in the buffer pointed to by <i>prgn</i>.


### -param pcElem [out]

Type: <b>ULONG*</b>

When this function returns, contains the count of <b>DOUBLE</b> elements extracted from the source <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

Returns <b>S_OK</b> if successful, or an error value otherwise, including the following:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TYPE_E_BUFFERTOOSMALL</b></dt>
</dl>
</td>
<td width="60%">
The source <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> contained more than <i>crgn</i> values.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> was not of the appropriate type.

</td>
</tr>
</table>
 




## -remarks



This helper function is used when the calling application expects a <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> to hold an array that consists of a fixed number of <b>DOUBLE</b> values.

If the source <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> has type VT_ARRAY | VT_DOUBLE, this function extracts up to <i>crgn</i> <b>DOUBLE</b> values and places them into the buffer pointed to by <i>prgn</i>.

If the <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> contains more elements than will fit into the <i>prgn</i> buffer, this function returns an error and sets *<i>pcElem</i> to 0.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="shell.VariantToDoubleArray">VariantToDoubleArray</a> to access a <b>DOUBLE</b> array stored in a <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>// VARIANT var;
// Assume variable var is initialized and valid.
DOUBLE rgDoubles[4]; // The application expects var to hold 4 DOUBLEs in an array.
ULONG cDoubles;

HRESULT hr = VariantToDoubleArray(var, rgDoubles, ARRAYSIZE(rgDoubles), &amp;cFlags);

if (SUCCEEDED(hr))
{
    if (cFlags == ARRAYSIZE(rgDoubles))
    {
        // The application got 4 DOUBLEs which are now stored in rgDoubles.
    }
    else
    {
        // The application got *pcElem DOUBLEs which are stored in the first 
        // *pcElem elements of rgDoubles.
    }
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="shell.InitVariantFromDoubleArray">InitVariantFromDoubleArray</a>



<a href="shell.PropVariantToDoubleVector">PropVariantToDoubleVector</a>



<a href="shell.VariantGetDoubleElem">VariantGetDoubleElem</a>



<a href="shell.VariantToDouble">VariantToDouble</a>



<a href="shell.VariantToDoubleArrayAlloc">VariantToDoubleArrayAlloc</a>
 

 

