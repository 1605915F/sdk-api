---
UID: NF:propvarutil.InitVariantFromInt32
title: InitVariantFromInt32 function
author: windows-sdk-content
description: Initializes a VARIANT structure with a 32-bit integer value.
old-location: properties\InitVariantFromInt32.htm
tech.root: properties
ms.assetid: b754149e-09e3-4420-b0e6-6e14ccbd9cff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitVariantFromInt32, InitVariantFromInt32 function [Windows Properties], _shell_InitVariantFromInt32, properties.InitVariantFromInt32, propvarutil/InitVariantFromInt32, shell.InitVariantFromInt32
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - InitVariantFromInt32
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitVariantFromInt32 function


## -description


Initializes a <a href="https://msdn.microsoft.com/en-us/library/ms221627(v=VS.85).aspx">VARIANT</a> structure with a 32-bit integer value.


## -parameters




### -param lVal [in]

Type: <b>LONG</b>

Source <b>LONG</b> value.


### -param pvar [out]

Type: <b>VARIANT*</b>

When this function returns, contains the initialized <a href="https://msdn.microsoft.com/en-us/library/ms221627(v=VS.85).aspx">VARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_I4 variant.

This is an inline function, with its source code provided in the header. It is not included in any .dll or .lib file.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="https://msdn.microsoft.com/en-us/library/Bb762329(v=VS.85).aspx">InitVariantFromInt32</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VARIANT var;

HRESULT hr = InitVariantFromInt32(3, &amp;var);

if (SUCCEEDED(hr))
{
    // var now is valid and has type VT_I4.
    VariantClear(&amp;propvar);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb762299(v=VS.85).aspx">InitPropVariantFromInt32</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb776608(v=VS.85).aspx">VariantToInt32</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb776611(v=VS.85).aspx">VariantToInt32WithDefault</a>
 

 

