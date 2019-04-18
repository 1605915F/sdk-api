---
UID: NF:dbghelp.SymGetLineFromAddr
title: SymGetLineFromAddr function (dbghelp.h)
author: windows-sdk-content
description: Locates the source line for the specified address.
old-location: base\symgetlinefromaddr64.htm
tech.root: Debug
ms.assetid: a1dad8e0-cd85-41f7-b0e3-e359be94c0ac
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SymGetLineFromAddr, SymGetLineFromAddr function, SymGetLineFromAddr64, SymGetLineFromAddr64 function, SymGetLineFromAddrW64, _win32_symgetlinefromaddr64, base.symgetlinefromaddr64, dbghelp/SymGetLineFromAddr, dbghelp/SymGetLineFromAddr64, dbghelp/SymGetLineFromAddrW64
ms.topic: function
req.header: dbghelp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SymGetLineFromAddrW64 (Unicode) and SymGetLineFromAddr64 (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dbghelp.lib
req.dll: Dbghelp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Dbghelp.dll
 - imagehlp.dll
api_name:
 - SymGetLineFromAddr64
 - SymGetLineFromAddr64
 - SymGetLineFromAddrW64
 - SymGetLineFromAddr
product: Windows
targetos: Windows
req.typenames: 
req.redist: DbgHelp.dll 5.1 or later
ms.custom: 19H1
---

# SymGetLineFromAddr function


## -description


Locates the source line for the specified address.


## -parameters




### -param hProcess [in]

A handle to the process that was originally passed to the 
      <a href="https://msdn.microsoft.com/fb1c98cb-6cd0-4218-aea4-384c24c66395">SymInitialize</a> function.


### -param dwAddr [in]

The address for which a line should be located. It is not necessary for the address to be on a line 
      boundary. If the address appears after the beginning of a line and before the end of the line, the line is 
      found.


### -param pdwDisplacement [out]

The displacement in bytes from the beginning of the line, or zero.


### -param Line [out]

A pointer to an <a href="https://msdn.microsoft.com/62124983-8381-4eb4-94f6-220b844aca45">IMAGEHLP_LINE64</a> 
      structure.


## -returns



If the function succeeds, the return value is <b>TRUE</b>.

If the function fails, the return value is <b>FALSE</b>. To retrieve extended error 
       information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The caller must allocate the <i>Line</i> buffer properly and fill in the required members 
    of the <a href="https://msdn.microsoft.com/62124983-8381-4eb4-94f6-220b844aca45">IMAGEHLP_LINE64</a> structure before 
    calling <b>SymGetLineFromAddr64</b>.

This function returns a pointer to a buffer that may be reused by another function. Therefore, be sure to copy 
    the data returned to another buffer immediately.

All DbgHelp functions, such as this one, are single threaded. Therefore, calls from more than one thread to 
    this function will likely result in unexpected behavior or memory corruption. To avoid this, you must synchronize 
    all concurrent calls from more than one thread to this function.

To call the Unicode version of this function, define <b>DBGHELP_TRANSLATE_TCHAR</b>. 
   <b>SymGetLineFromAddrW64</b> is defined as follows in 
   Dbghelp.h.
   


```cpp
BOOL
IMAGEAPI
SymGetLineFromAddrW64(
    _In_ HANDLE hProcess,
    _In_ DWORD64 dwAddr,
    _Out_ PDWORD pdwDisplacement,
    _Out_ PIMAGEHLP_LINEW64 Line
    );

#ifdef DBGHELP_TRANSLATE_TCHAR
 #define SymGetLineFromAddr64   SymGetLineFromAddrW64
#endif
```


This function supersedes the <b>SymGetLineFromAddr</b> function. For more information, see 
<a href="https://msdn.microsoft.com/34ec8cd3-3260-441d-b55f-4ea21c736eb1">Updated Platform Support</a>. <b>SymGetLineFromAddr</b> is defined as follows in Dbghelp.h. 


```cpp
#if !defined(_IMAGEHLP_SOURCE_) && defined(_IMAGEHLP64)
#define SymGetLineFromAddr SymGetLineFromAddr64
#define SymGetLineFromAddrW SymGetLineFromAddrW64
#else
BOOL
IMAGEAPI
SymGetLineFromAddr(
    _In_ HANDLE hProcess,
    _In_ DWORD dwAddr,
    _Out_ PDWORD pdwDisplacement,
    _Out_ PIMAGEHLP_LINE Line
    );

BOOL
IMAGEAPI
SymGetLineFromAddrW(
    _In_ HANDLE hProcess,
    _In_ DWORD dwAddr,
    _Out_ PDWORD pdwDisplacement,
    _Out_ PIMAGEHLP_LINEW Line
    );
#endif
```



#### Examples

For an example, see 
     <a href="https://msdn.microsoft.com/63dfadea-b0c4-4050-add8-d1f3aef7a495">Retrieving Symbol Information by Address</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/7b28f70b-2d97-4cc2-8064-dfb806f9cffa">DbgHelp Functions</a>



<a href="https://msdn.microsoft.com/62124983-8381-4eb4-94f6-220b844aca45">IMAGEHLP_LINE64</a>



<a href="https://msdn.microsoft.com/cb8870f6-1bae-40df-842e-ec3ca0167691">SymGetLineFromName64</a>



<a href="https://msdn.microsoft.com/fb1c98cb-6cd0-4218-aea4-384c24c66395">SymInitialize</a>
 

 

