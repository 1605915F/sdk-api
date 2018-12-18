---
UID: NF:propvarutil.InitVariantFromResource
title: InitVariantFromResource function
author: windows-sdk-content
description: Initializes a VARIANT structure based on a string resource imbedded in an executable file.
old-location: properties\InitVariantFromResource.htm
tech.root: properties
ms.assetid: ae309a04-7b21-46ef-b481-2593dc162e19
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitVariantFromResource, InitVariantFromResource function [Windows Properties], _shell_InitVariantFromResource, properties.InitVariantFromResource, propvarutil/InitVariantFromResource, shell.InitVariantFromResource
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
 - InitVariantFromResource
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitVariantFromResource function


## -description


Initializes a <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure based on a string resource imbedded in an executable file.


## -parameters




### -param hinst [in]

Type: <b>HINSTANCE</b>

Handle to an instance of the module whose executable file contains the string resource.


### -param id [in]

Type: <b>UINT</b>

Integer identifier of the string to be loaded.


### -param pvar [out]

Type: <b>VARIANT*</b>

When this function returns, contains the initialized <a href="e305240e-9e11-4006-98cc-26f4932d2118">VARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_BSTR variant. If the resource does not exist, this function initializes the VARIANT as VT_EMPTY and returns a failure code.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="shell.InitVariantFromResource">InitVariantFromResource</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>// HINSTANCE hinst;
// UINT id;
// Assume variables hinst and id are initialized and valid.
VARIANT var;

HRESULT hr = InitVariantFromResource(hinst, id, &amp;var);

if (SUCCEEDED(hr))
{
    // var now is valid and has type VT_BSTR.
    VariantClear(&amp;var);
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="shell.InitPropVariantFromResource">InitPropVariantFromResource</a>



<a href="shell.InitVariantFromString">InitVariantFromString</a>



<a href="https://msdn.microsoft.com/9d878af7-a7b1-4d24-89ff-c567e4a8accd">LoadString</a>



<a href="shell.VariantToString">VariantToString</a>



<a href="shell.VariantToStringWithDefault">VariantToStringWithDefault</a>
 

 

