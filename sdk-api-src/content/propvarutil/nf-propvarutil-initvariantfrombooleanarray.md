---
UID: NF:propvarutil.InitVariantFromBooleanArray
title: InitVariantFromBooleanArray function
author: windows-sdk-content
description: Initializes a VARIANT structure from an array of Boolean values.
old-location: properties\InitVariantFromBooleanArray.htm
tech.root: properties
ms.assetid: 50780131-c0ed-443b-86e8-deb996a5c98e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitVariantFromBooleanArray, InitVariantFromBooleanArray function [Windows Properties], _shell_InitVariantFromBooleanArray, properties.InitVariantFromBooleanArray, propvarutil/InitVariantFromBooleanArray, shell.InitVariantFromBooleanArray
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
 - InitVariantFromBooleanArray
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitVariantFromBooleanArray function


## -description


Initializes a <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure from an array of Boolean values.


## -parameters




### -param prgf [in]

Type: <b>const BOOL*</b>

Pointer to source array of Boolean values.


### -param cElems [in]

Type: <b>ULONG</b>

The number of elements in the array.


### -param pvar [out]

Type: <b>VARIANT*</b>

When this function returns, contains the initialized <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_ARRAY | VT_BOOL variant.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="shell.InitVariantFromBooleanArray">InitVariantFromBooleanArray</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>BOOL rgFlags[] = {TRUE, FALSE};
VARIANT var;

HRESULT hr = InitVariantFromBooleanArray(rgFlags, ARRAYSIZE(rgFlags), &amp;var);

if (SUCCEEDED(hr))
{
    // var now is valid and has type VT_ARRAY | VT_BOOL.
    VariantClear(&amp;propvar);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="shell.InitPropVariantFromBooleanVector">InitPropVariantFromBooleanVector</a>



<a href="shell.VariantToBooleanArray">VariantToBooleanArray</a>
 

 

