---
UID: NF:propvarutil.InitPropVariantFromDouble
title: InitPropVariantFromDouble function
author: windows-sdk-content
description: Initializes a PROPVARIANT structure based on a specified double value.
old-location: properties\InitPropVariantFromDouble.htm
tech.root: properties
ms.assetid: aeae9091-3b1e-4112-8f50-79d77cb891c4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitPropVariantFromDouble, InitPropVariantFromDouble function [Windows Properties], properties.InitPropVariantFromDouble, propvarutil/InitPropVariantFromDouble, shell.InitPropVariantFromDouble, shell_InitPropVariantFromDouble
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Propvarutil.h
api_name:
 - InitPropVariantFromDouble
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitPropVariantFromDouble function


## -description


Initializes a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure based on a specified <b>double</b> value.


## -parameters




### -param dblVal [in]

Type: <b>DOUBLE</b>

The source <b>double</b> value.


### -param ppropvar [out]

Type: <b><a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a>*</b>

When this function returns, contains the initialized <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_R8 propvariant.

This is an inline function, with its source code provided in the header. It is not included in any .dll or .lib file.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="shell.InitPropVariantFromDouble">InitPropVariantFromDouble</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>PROPVARIANT propvar;

HRESULT hr = InitPropVariantFromDouble(3.1415, &amp;propvar);

if (SUCCEEDED(hr))
{
    // propvar now is valid and has type VT_R8.
 
    PropVariantClear(&amp;propvar);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="shell.InitPropVariantFromDoubleVector">InitPropVariantFromDoubleVector</a>



<a href="shell.InitVariantFromDouble">InitVariantFromDouble</a>



<a href="shell.PropVariantToDouble">PropVariantToDouble</a>



<a href="shell.PropVariantToDoubleWithDefault">PropVariantToDoubleWithDefault</a>
 

 

