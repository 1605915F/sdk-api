---
UID: NF:dbghelp.SymGetSearchPathW
title: SymGetSearchPathW function
author: windows-sdk-content
description: Retrieves the symbol search path for the specified process.
old-location: base\symgetsearchpath.htm
tech.root: debug
ms.assetid: aa8c8450-ee67-4614-98a1-5feebdd3a788
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SymGetSearchPath, SymGetSearchPath function, SymGetSearchPathW, _win32_symgetsearchpath, base.symgetsearchpath, dbghelp/SymGetSearchPath, dbghelp/SymGetSearchPathW
ms.topic: function
req.header: dbghelp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SymGetSearchPathW (Unicode) and SymGetSearchPath (ANSI)
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
 - SymGetSearchPath
 - SymGetSearchPath
 - SymGetSearchPathW
product: Windows
targetos: Windows
req.typenames: 
req.redist: DbgHelp.dll 5.1 or later
---

# SymGetSearchPathW function


## -description


Retrieves the symbol search path for the specified process.


## -parameters




### -param hProcess [in]

A handle to the process that was originally passed to the 
<a href="https://msdn.microsoft.com/fb1c98cb-6cd0-4218-aea4-384c24c66395">SymInitialize</a> function.


### -param SearchPath [out]

A pointer to the buffer that receives the symbol search path.


### -param SearchPathLength [in]

The size of the <i>SearchPath</i> buffer, in characters.


## -returns



If the function succeeds, the return value is <b>TRUE</b>.

If the function fails, the return value is <b>FALSE</b>. To retrieve extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The 
<b>SymGetSearchPath</b> function copies the symbol search path for the specified process into the <i>SearchPath</i> buffer. If the function fails, the contents of the buffer are undefined.

To specify a symbol search path for the process, use the 
<a href="https://msdn.microsoft.com/564ba1f6-65c6-4c45-bdbf-41ef0dd8a39d">SymSetSearchPath</a> function.

All DbgHelp functions, such as this one, are single threaded. Therefore, calls from more than one thread to this function will likely result in unexpected behavior or memory corruption. To avoid this, you must synchronize all concurrent calls from more than one thread to this function.

To call the Unicode version of this function, define DBGHELP_TRANSLATE_TCHAR.




## -see-also




<a href="https://msdn.microsoft.com/7b28f70b-2d97-4cc2-8064-dfb806f9cffa">DbgHelp Functions</a>



<a href="https://msdn.microsoft.com/fb1c98cb-6cd0-4218-aea4-384c24c66395">SymInitialize</a>



<a href="https://msdn.microsoft.com/564ba1f6-65c6-4c45-bdbf-41ef0dd8a39d">SymSetSearchPath</a>
 

 

