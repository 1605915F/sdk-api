---
UID: NF:propvarutil.InitVariantFromDispatch
title: InitVariantFromDispatch function (propvarutil.h)
author: windows-sdk-content
description: Initializes a VARIANT structure based on an instance of an IDispatch object.
old-location: properties\InitVariantFromDispatch.htm
tech.root: properties
ms.assetid: d42c48b5-cfd9-4de8-b0aa-b108d242e2e9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InitVariantFromDispatch, InitVariantFromDispatch function [Windows Properties], _shell_InitVariantFromDispatch, properties.InitVariantFromDispatch, propvarutil/InitVariantFromDispatch, shell.InitVariantFromDispatch
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
 - InitVariantFromDispatch
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Desktop Search (WDS) 3.0
---

# InitVariantFromDispatch function


## -description


Initializes a <a href="https://msdn.microsoft.com/en-us/library/ms221627(v=VS.85).aspx">VARIANT</a> structure based on an instance of an <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> object.


## -parameters




### -param pdisp [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>*</b>

Pointer to the source <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>.


### -param pvar [out]

Type: <b>VARIANT*</b>

When this function returns, contains the initialized <a href="https://msdn.microsoft.com/en-us/library/ms221627(v=VS.85).aspx">VARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Creates a <b>VT_DISPATCH</b> variant.

This is an inline function, with its source code provided in the header. It is not included in any .dll or .lib file.


#### Examples

The following example, to be included as part of a larger program, demonstrates how to use <a href="https://msdn.microsoft.com/en-us/library/Bb762319(v=VS.85).aspx">InitVariantFromDispatch</a>.


```cpp
// IDispatch *pDispatch;
// Assume variable pDispatch is initialized and valid.
VARIANT var;

HRESULT hr = InitVariantFromDispatch(pDispatch, &var);

if (SUCCEEDED(hr))
{
    // var now is valid and has type VT_DISPATCH.
    VariantClear(&propvar);
}
```




