---
UID: NF:propvarutil.InitPropVariantFromGUIDAsBuffer
title: InitPropVariantFromGUIDAsBuffer function (propvarutil.h)
author: windows-sdk-content
description: Initializes a PROPVARIANT structure based on a GUID. The structure is initialized as VT_VECTOR | VT_UI1.
old-location: properties\InitPropVariantFromGUIDAsBuffer.htm
tech.root: properties
ms.assetid: 9ff3ec09-3314-4830-b970-b33f5a53d66c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: InitPropVariantFromGUIDAsBuffer, InitPropVariantFromGUIDAsBuffer function [Windows Properties], properties.InitPropVariantFromGUIDAsBuffer, propvarutil/InitPropVariantFromGUIDAsBuffer, shell.InitPropVariantFromGUIDAsBuffer, shell_InitPropVariantFromGUIDAsBuffer
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
 - InitPropVariantFromGUIDAsBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitPropVariantFromGUIDAsBuffer function


## -description


Initializes a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure based on a <b>GUID</b>. The structure is initialized as VT_VECTOR | VT_UI1.


## -parameters




### -param guid [in]

Type: <b>REFGUID</b>

Reference to the source <b>GUID</b>.


### -param ppropvar [out]

Type: <b><a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a>*</b>

When this function returns, contains the initialized <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_VECTOR | VT_UI1 propvariant.

This is an inline function, with its source code provided in the header. It is not included in any .dll or .lib file.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <b>InitPropVariantFromGUIDAsBuffer</b>.


```cpp
PROPVARIANT propvar;

HRESULT hr = InitPropVariantFromGUIDAsBuffer(FMTID_DocSummaryInformation, &propvar);

if (SUCCEEDED(hr))
{
    // propvar now is valid and has type VT_VECTOR | VT_UI1.
 
    PropVariantClear(&propvar);
}
```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb762290(v=VS.85).aspx">InitPropVariantFromCLSID</a>



<a href="https://msdn.microsoft.com/bcc343f7-741f-4cdd-bd2f-ae4786faab0e">InitPropVariantFromGUIDAsString</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb762325(v=VS.85).aspx">InitVariantFromGUIDAsBuffer</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb776536(v=VS.85).aspx">PropVariantToBuffer</a>
 

 

