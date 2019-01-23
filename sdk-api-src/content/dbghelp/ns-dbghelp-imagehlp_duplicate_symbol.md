---
UID: NS:dbghelp._IMAGEHLP_DUPLICATE_SYMBOL
title: IMAGEHLP_DUPLICATE_SYMBOL
author: windows-sdk-content
description: Contains duplicate symbol information.
old-location: base\imagehlp_duplicate_symbol64_str.htm
tech.root: debug
ms.assetid: 47ef96d5-94ba-487c-8678-59ddd18ad449
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PIMAGEHLP_DUPLICATE_SYMBOL, IMAGEHLP_DUPLICATE_SYMBOL, IMAGEHLP_DUPLICATE_SYMBOL structure, IMAGEHLP_DUPLICATE_SYMBOL64, IMAGEHLP_DUPLICATE_SYMBOL64 structure, PIMAGEHLP_DUPLICATE_SYMBOL64, PIMAGEHLP_DUPLICATE_SYMBOL64 structure pointer, _IMAGEHLP_DUPLICATE_SYMBOL64, _win32_imagehlp_duplicate_symbol64_str, base.imagehlp_duplicate_symbol64_str, dbghelp/IMAGEHLP_DUPLICATE_SYMBOL64, dbghelp/PIMAGEHLP_DUPLICATE_SYMBOL64"
ms.topic: struct
req.header: dbghelp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - DbgHelp.h
api_name:
 - IMAGEHLP_DUPLICATE_SYMBOL64
 - IMAGEHLP_DUPLICATE_SYMBOL
product: Windows
targetos: Windows
req.typenames: IMAGEHLP_DUPLICATE_SYMBOL, *PIMAGEHLP_DUPLICATE_SYMBOL
req.redist: DbgHelp.dll 5.1 or later
---

# IMAGEHLP_DUPLICATE_SYMBOL structure


## -description


Contains duplicate symbol information.


## -struct-fields




### -field SizeOfStruct

The size of the structure, in bytes. The caller must set this member to <code>sizeof(IMAGEHLP_DUPLICATE_SYMBOL64)</code>.


### -field NumberOfDups

The number of duplicate symbols.


### -field Symbol

A pointer to an array of symbols (
<a href="https://msdn.microsoft.com/7b39281a-c34b-47ae-a3ff-5f0a7a66a588">IMAGEHLP_SYMBOL64</a> structures). The number of entries in the array is specified by the <b>NumberOfDups</b> member.


### -field SelectedSymbol

The index into the symbol array for the selected symbol.


## -remarks



This structure supersedes the <b>IMAGEHLP_DUPLICATE_SYMBOL</b> structure. For more information, see 
<a href="https://msdn.microsoft.com/34ec8cd3-3260-441d-b55f-4ea21c736eb1">Updated Platform Support</a>. <b>IMAGEHLP_DUPLICATE_SYMBOL</b> is defined as follows in DbgHelp.h. 


```cpp
#if !defined(_IMAGEHLP_SOURCE_) && defined(_IMAGEHLP64)
#define IMAGEHLP_DUPLICATE_SYMBOL IMAGEHLP_DUPLICATE_SYMBOL64
#define PIMAGEHLP_DUPLICATE_SYMBOL PIMAGEHLP_DUPLICATE_SYMBOL64
#else
typedef struct _IMAGEHLP_DUPLICATE_SYMBOL {
    DWORD            SizeOfStruct;
    DWORD            NumberOfDups; 
    PIMAGEHLP_SYMBOL Symbol; 
    DWORD            SelectedSymbol; 
} IMAGEHLP_DUPLICATE_SYMBOL, *PIMAGEHLP_DUPLICATE_SYMBOL;
#endif
```





## -see-also




<a href="https://msdn.microsoft.com/7b39281a-c34b-47ae-a3ff-5f0a7a66a588">IMAGEHLP_SYMBOL64</a>



<a href="https://msdn.microsoft.com/f3ba952b-ecc5-4235-a806-00c82d40e611">SymRegisterCallbackProc64</a>
 

 

