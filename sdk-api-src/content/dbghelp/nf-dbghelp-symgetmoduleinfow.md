---
UID: NF:dbghelp.SymGetModuleInfoW
title: SymGetModuleInfoW function (dbghelp.h)
author: windows-sdk-content
description: Retrieves the module information of the specified module.
old-location: base\symgetmoduleinfo64.htm
tech.root: Debug
ms.assetid: e8057cb5-3331-4460-b07c-4338a57024be
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SymGetModuleInfo, SymGetModuleInfo function, SymGetModuleInfo64, SymGetModuleInfo64 function, SymGetModuleInfoW, SymGetModuleInfoW64, _win32_symgetmoduleinfo64, base.symgetmoduleinfo64, dbghelp/SymGetModuleInfo, dbghelp/SymGetModuleInfo64, dbghelp/SymGetModuleInfoW, dbghelp/SymGetModuleInfoW64
ms.topic: function
req.header: dbghelp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SymGetModuleInfoW64 (Unicode) and SymGetModuleInfo64 (ANSI)
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
api_name:
 - SymGetModuleInfo64
 - SymGetModuleInfo64
 - SymGetModuleInfoW64
 - SymGetModuleInfo
 - SymGetModuleInfoW
product: Windows
targetos: Windows
req.typenames: 
req.redist: DbgHelp.dll 5.1 or later
ms.custom: 19H1
---

# SymGetModuleInfoW function


## -description


Retrieves the module information of the specified module.


## -parameters




### -param hProcess [in]

A handle to the process that was originally passed to the 
<a href="https://msdn.microsoft.com/fb1c98cb-6cd0-4218-aea4-384c24c66395">SymInitialize</a> function.


#### - dwAddr [in]

The virtual address that is contained in one of the modules loaded by the 
<a href="https://msdn.microsoft.com/be50588b-066b-42ab-ba81-7537c811676f">SymLoadModule64</a> function


### -param ModuleInfo [out]

A pointer to an 
<a href="https://msdn.microsoft.com/3cc7a678-561b-4af8-8cf0-5cf6ebc0cb26">IMAGEHLP_MODULE64</a> structure. The <b>SizeOfStruct</b> member must be set to the size of the 
<b>IMAGEHLP_MODULE64</b> structure. An invalid value will result in an error.


## -returns



If the function succeeds, the return value is <b>TRUE</b>.

If the function fails, the return value is <b>FALSE</b>. To retrieve extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The module table is searched for a module that contains the <i>dwAddr</i>. The module is located based on the load address and size of each module. If a valid module is found, the <i>ModuleInfo</i> parameter is filled with the information about the module.

The size of the <a href="https://msdn.microsoft.com/3cc7a678-561b-4af8-8cf0-5cf6ebc0cb26">IMAGEHLP_MODULE64</a> structure used by this function has changed over the years.  If a version of DbgHelp.dll is called that is older than the DbgHelp.h used to compile the calling code, then this function may fail with an error code of <b>ERROR_INVALID_PARAMETER</b>.  This most commonly occurs when the system version (%WinDir%\System32\DbgHelp.dll) is called.  Code that calls the system version of DbgHelp.dll must be compiled using the appropriate SDK for that Windows release or the SDK for a previous release.  

The recommended model is to redistribute the required version of DbgHelp.dll along with the calling software.  This allows the caller to use the most robust versions of DbgHelp.dll as well as a simplifying upgrades.  The most recent version of DbgHelp.dll can always be found in the <a href="http://go.microsoft.com/fwlink/p/?linkid=153784 ">Debugging Tools for Windows</a> package.  As a general rule, code that is compiled to work with older versions will always work with newer versions.

All DbgHelp functions, such as this one, are single threaded. Therefore, calls from more than one thread to this function will likely result in unexpected behavior or memory corruption. To avoid this, you must synchronize all concurrent calls from more than one thread to this function.

To call the Unicode version of this function, define <b>DBGHELP_TRANSLATE_TCHAR</b>. <b>SymGetModuleInfoW64</b> is defined as follows in DbgHelp.h. 


```cpp

BOOL
IMAGEAPI
SymGetModuleInfoW64(
    __in HANDLE hProcess,
    __in DWORD64 qwAddr,
    __out PIMAGEHLP_MODULEW64 ModuleInfo
    );

#ifdef DBGHELP_TRANSLATE_TCHAR
#define SymGetModuleInfo64   SymGetModuleInfoW64
#endif
```


This function supersedes the <b>SymGetModuleInfo</b> function. For more information, see 
<a href="https://msdn.microsoft.com/34ec8cd3-3260-441d-b55f-4ea21c736eb1">Updated Platform Support</a>. <b>SymGetModuleInfo</b> is defined as follows in DbgHelp.h. 


```cpp
#if !defined(_IMAGEHLP_SOURCE_) && defined(_IMAGEHLP64)
#define SymGetModuleInfo   SymGetModuleInfo64
#define SymGetModuleInfoW  SymGetModuleInfoW64
#else
BOOL
IMAGEAPI
SymGetModuleInfo(
    __in HANDLE hProcess,
    __in DWORD dwAddr,
    __out PIMAGEHLP_MODULE ModuleInfo
    );

BOOL
IMAGEAPI
SymGetModuleInfoW(
    __in HANDLE hProcess,
    __in DWORD dwAddr,
    __out PIMAGEHLP_MODULEW ModuleInfo
    );
#endif
```





## -see-also




<a href="https://msdn.microsoft.com/7b28f70b-2d97-4cc2-8064-dfb806f9cffa">DbgHelp Functions</a>



<a href="https://msdn.microsoft.com/3cc7a678-561b-4af8-8cf0-5cf6ebc0cb26">IMAGEHLP_MODULE64</a>



<a href="https://msdn.microsoft.com/fb1c98cb-6cd0-4218-aea4-384c24c66395">SymInitialize</a>



<a href="https://msdn.microsoft.com/be50588b-066b-42ab-ba81-7537c811676f">SymLoadModule64</a>
 

 

