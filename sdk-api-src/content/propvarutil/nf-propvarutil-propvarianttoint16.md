---
UID: NF:propvarutil.PropVariantToInt16
title: PropVariantToInt16 function
author: windows-sdk-content
description: Extracts an Int16 property value of a PROPVARIANT structure.
old-location: properties\PropVariantToInt16.htm
tech.root: properties
ms.assetid: 32070620-bae2-4465-8b11-b88adb6cb365
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PropVariantToInt16, PropVariantToInt16 function [Windows Properties], properties.PropVariantToInt16, propvarutil/PropVariantToInt16, shell.PropVariantToInt16, shell_PropVariantToInt16
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
 - PropVariantToInt16
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# PropVariantToInt16 function


## -description


Extracts an Int16 property value of a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


## -parameters




### -param propvarIn [in]

Type: <b>REFPROPVARIANT</b>

Reference to a source <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


### -param piRet [out]

Type: <b>SHORT*</b>

When this function returns, contains the extracted property value if one exists; otherwise, 0.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This helper function is used in places where the calling application expects a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> to hold an Int16 value. For instance, an application obtaining values from a property store can use this to safely extract the Int16 value for Int16 properties.

If the source <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> has type <b>VT_I2</b>, this helper function extracts the Int16 value. Otherwise, it attempts to convert the value in the <b>PROPVARIANT</b> structure into an Int16. If a conversion is not possible, <a href="shell.PropVariantToInt16">PropVariantToInt16</a> will return a failure code and set <i>piRet</i> to 0. See <a href="shell.PropVariantChangeType">PropVariantChangeType</a> for a list of possible conversions. Of note, VT_EMPTY is successfully converted to 0.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="shell.PropVariantToInt16">PropVariantToInt16</a> to access an Int16 value in a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a>.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>// IPropertyStore *ppropstore;

// Assume variable ppropstore is initialized and valid

PROPVARIANT propvar = {0};

HRESULT hr = ppropstore-&gt;GetValue(PKEY_Image_ResolutionUnit, &amp;propvar);

if (SUCCEEDED(hr))

{

     // PKEY_Image_ResolutionUnit is expected to produce a VT_I2 or VT_EMPTY value.

     // PropVariantToInt16 will convert VT_EMPTY to 0.

     INT16 iUnit;

     hr = PropVariantToInt16(propvar, &amp; iUnit);

     if (SUCCEEDED(hr))

     {

             // iUnit is now valid

     }

     else

     {

             // iUnit is always 0

     }

     PropVariantClear(&amp;propvar);

}</pre>
</td>
</tr>
</table></span></div>


