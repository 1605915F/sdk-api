---
UID: NF:propvarutil.InitPropVariantFromCLSID
title: InitPropVariantFromCLSID function (propvarutil.h)
author: windows-sdk-content
description: Initializes a PROPVARIANT structure based on a class identifier (CLSID).
old-location: properties\InitPropVariantFromCLSID.htm
tech.root: properties
ms.assetid: a48a8927-2718-4f9c-96f2-ab370206550b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitPropVariantFromCLSID, InitPropVariantFromCLSID function [Windows Properties], properties.InitPropVariantFromCLSID, propvarutil/InitPropVariantFromCLSID, shell.InitPropVariantFromCLSID, shell_InitPropVariantFromCLSID
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
 - InitPropVariantFromCLSID
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitPropVariantFromCLSID function


## -description


Initializes a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure based on a class identifier (CLSID).


## -parameters




### -param clsid [in]

Type: <b>REFCLSID</b>

Reference to the CLSID.


### -param ppropvar [out]

Type: <b><a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a>*</b>

When this function returns, contains the initialized <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a VT_CLSID propvariant.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="https://msdn.microsoft.com/en-us/library/Bb762290(v=VS.85).aspx">InitPropVariantFromCLSID</a>.


```cpp
PROPVARIANT propvar;

HRESULT hr = InitPropVariantFromCLSID(CLSID_PropertySystem, &propvar);

if (SUCCEEDED(hr))
{
    // propvar now is valid and has type VT_CLSID.
 
    PropVariantClear(&propvar);
}
```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb762325(v=VS.85).aspx">InitVariantFromGUIDAsBuffer</a>



<a href="https://msdn.microsoft.com/2a78257a-a8ce-45e8-aea2-dfa9f380528a">InitVariantFromGUIDAsString</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb776537(v=VS.85).aspx">PropVariantToCLSID</a>
 

 

