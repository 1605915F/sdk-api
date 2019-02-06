---
UID: NF:minidumpapiset.MiniDumpWriteDump
title: MiniDumpWriteDump function
author: windows-sdk-content
description: Writes user-mode minidump information to the specified file.
old-location: base\minidumpwritedump.htm
tech.root: Debug
ms.assetid: b476023d-0e93-4d76-9ba8-ce5766c9ac51
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MiniDumpWriteDump, MiniDumpWriteDump function, _win32_minidumpwritedump, base.minidumpwritedump, minidumpapiset/MiniDumpWriteDump
ms.topic: function
req.header: minidumpapiset.h
req.include-header: Dbghelp.h
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
req.lib: Dbghelp.lib
req.dll: Dbghelp.dll; Dbgcore.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Dbghelp.dll
 - Dbgcore.dll
 - API-MS-Win-Core-Debug-MiniDump-L1-1-0.dll
 - DbgCore.dll
api_name:
 - MiniDumpWriteDump
product: Windows
targetos: Windows
req.typenames: 
req.redist: DbgHelp.dll and Dbgcore.dll
---

# MiniDumpWriteDump function


## -description


Writes user-mode minidump information to the specified file.


## -parameters




### -param hProcess [in]

A handle to the process for which the information is to be generated.

This handle must have <b>PROCESS_QUERY_INFORMATION</b> and 
       <b>PROCESS_VM_READ</b> access to the process. If handle information is to be collected then 
       <b>PROCESS_DUP_HANDLE</b> access is also required. For more information, see 
       <a href="https://msdn.microsoft.com/508a17c4-88cd-431a-a102-00180a7f7ab5">Process Security and Access Rights</a>. 
       The caller must also be able to get <b>THREAD_ALL_ACCESS</b> access to the threads in the 
       process. For more information, see 
       <a href="https://msdn.microsoft.com/72709446-5c59-4fac-8dc8-7912906ecc85">Thread Security and Access Rights</a>.


### -param ProcessId [in]

The identifier of the process for which the information is to be generated.


### -param hFile [in]

A handle to the file in which the information is to be written.


### -param DumpType [in]

The type of information to be generated. This parameter can be one or more of the values from the 
      <a href="https://msdn.microsoft.com/89ae3a75-5f02-4c5e-9d72-95fb8ef94985">MINIDUMP_TYPE</a> enumeration.


### -param ExceptionParam [in]

A pointer to a 
      <a href="https://msdn.microsoft.com/en-us/library/ms680366(v=VS.85).aspx">MINIDUMP_EXCEPTION_INFORMATION</a> 
      structure describing the client exception that caused the minidump to be generated. If the value of this 
      parameter is <b>NULL</b>, no exception information is included in the minidump file.


### -param UserStreamParam [in]

A pointer to a 
      <a href="https://msdn.microsoft.com/en-us/library/ms680524(v=VS.85).aspx">MINIDUMP_USER_STREAM_INFORMATION</a> 
      structure. If the value of this parameter is <b>NULL</b>, no user-defined information is 
      included in the minidump file.


### -param CallbackParam [in]

A pointer to a 
      <a href="https://msdn.microsoft.com/en-us/library/ms680361(v=VS.85).aspx">MINIDUMP_CALLBACK_INFORMATION</a> 
      structure that specifies a callback routine which is to receive extended minidump information. If the value of 
      this parameter is <b>NULL</b>, no callbacks are performed.


## -returns



If the function succeeds, the return value is <b>TRUE</b>; otherwise, the return value is 
       <b>FALSE</b>. To retrieve extended error information, call 
       <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. Note that the last error will be an 
       <b>HRESULT</b> value.

If the operation is canceled, the last error code is 
       <code>HRESULT_FROM_WIN32(ERROR_CANCELLED)</code>.




## -remarks



The <a href="https://msdn.microsoft.com/8dc95b0a-6aee-4c38-ab25-a800153bbe91">MiniDumpCallback</a> function receives extended 
    minidump information from <b>MiniDumpWriteDump</b>. It also 
    provides a way for the caller to determine the granularity of information written to the minidump file, as the 
    callback function can filter the default information.

<b>MiniDumpWriteDump</b> should be called from a 
    separate process if at all possible, rather than from within the target process being dumped.  This is especially 
    true when the target process is already not stable.  For example, if it just crashed.  A loader deadlock is one of 
    many potential side effects of calling 
    <b>MiniDumpWriteDump</b> from within the target 
    process.

<b>MiniDumpWriteDump</b> may not produce a valid  stack 
    trace for the calling thread. To work around this problem, you must capture the state of the calling thread before 
    calling <b>MiniDumpWriteDump</b> and use it as the 
    <i>ExceptionParam</i> parameter. One way to do this is to force  an exception inside a 
    <b>__try</b>/<b>__except</b> block and use the 
    <a href="https://msdn.microsoft.com/57e8cb3a-1b11-45b9-9676-3b6dc600d225">EXCEPTION_POINTERS</a> information provided by 
    <a href="https://msdn.microsoft.com/e982794a-d5f1-4fb4-a2b9-aa8da18cb8ae">GetExceptionInformation</a>. Alternatively, you 
    can call the function from a new worker thread and filter this worker thread from the dump.

All DbgHelp functions, such as this one, are single threaded. Therefore, calls from more than one thread to 
    this function will likely result in unexpected behavior or memory corruption. To avoid this, you must synchronize 
    all concurrent calls from more than one thread to this function.




## -see-also




<a href="https://msdn.microsoft.com/7b28f70b-2d97-4cc2-8064-dfb806f9cffa">DbgHelp Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/ms680361(v=VS.85).aspx">MINIDUMP_CALLBACK_INFORMATION</a>



<a href="https://msdn.microsoft.com/en-us/library/ms680366(v=VS.85).aspx">MINIDUMP_EXCEPTION_INFORMATION</a>



<a href="https://msdn.microsoft.com/en-us/library/ms680524(v=VS.85).aspx">MINIDUMP_USER_STREAM_INFORMATION</a>



<a href="https://msdn.microsoft.com/8dc95b0a-6aee-4c38-ab25-a800153bbe91">MiniDumpCallback</a>



<a href="https://msdn.microsoft.com/56df69aa-55b6-451b-a003-3ee88dc934f9">MiniDumpReadDumpStream</a>
 

 

