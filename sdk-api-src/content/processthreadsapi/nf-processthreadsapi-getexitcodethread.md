---
UID: NF:processthreadsapi.GetExitCodeThread
title: GetExitCodeThread function (processthreadsapi.h)
author: windows-sdk-content
description: Retrieves the termination status of the specified thread.
old-location: base\getexitcodethread.htm
tech.root: ProcThread
ms.assetid: 67482c3d-b845-4c0f-8aa1-0e3cf8cb5127
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetExitCodeThread, GetExitCodeThread function, _win32_getexitcodethread, base.getexitcodethread, processthreadsapi/GetExitCodeThread, winbase/GetExitCodeThread
ms.topic: function
req.header: processthreadsapi.h
req.include-header: Windows Server 2003, Windows Vista, Windows 7, Windows Server 2008  Windows Server 2008 R2, Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib; WindowsPhoneCore.lib on Windows Phone 8.1
req.dll: Kernel32.dll; KernelBase.dll on Windows Phone 8.1
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
 - KernelBase.dll
 - API-MS-Win-Core-ProcessThreads-l1-1-0.dll
 - MinKernelBase.dll
 - API-MS-Win-Core-ProcessThreads-l1-1-1.dll
 - API-MS-Win-Core-ProcessThreads-l1-1-2.dll
 - api-ms-win-downlevel-kernel32-l1-1-0.dll
 - API-MS-Win-Core-ProcessThreads-L1-1-3.dll
api_name:
 - GetExitCodeThread
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetExitCodeThread function


## -description


Retrieves the termination status of the specified thread.


## -parameters




### -param hThread [in]

A handle to the thread.

The handle must have the <b>THREAD_QUERY_INFORMATION</b> or <b>THREAD_QUERY_LIMITED_INFORMATION</b> access right. For more information, see 
<a href="https://msdn.microsoft.com/72709446-5c59-4fac-8dc8-7912906ecc85">Thread Security and Access Rights</a>.

<b>Windows Server 2003 and Windows XP:  </b>The handle must have the <b>THREAD_QUERY_INFORMATION</b> access right.


### -param lpExitCode [out]

A pointer to a variable to receive the thread termination status. For more information, see Remarks.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



This function returns immediately. If the specified thread has not terminated and the function succeeds, the status returned is <b>STILL_ACTIVE</b>. If the thread has terminated and the function succeeds, the status returned is one of the following values:

<ul>
<li>The exit value specified in the 
<a href="https://msdn.microsoft.com/e7f6d054-c535-4521-a3b4-800a9174732f">ExitThread</a> or 
<a href="https://msdn.microsoft.com/ae1ad0f3-67df-4573-af22-7086f0470361">TerminateThread</a> function.</li>
<li>The return value from the thread function.</li>
<li>The exit value of the thread's process.</li>
</ul>
<div class="alert"><b>Important</b>  The <b>GetExitCodeThread</b> function returns a valid error code defined by the application only after the thread terminates. Therefore, an application should not use <b>STILL_ACTIVE</b> (259) as an error code. If a thread returns <b>STILL_ACTIVE</b> (259) as an error code, applications that test for this value could interpret it to mean that the thread is still running and continue to test for the completion of the thread after the thread has terminated, which could put the application into an infinite loop. To avoid this problem, callers should call the <b>GetExitCodeThread</b> function only after the thread has been confirmed to have exited. Use the <a href="https://docs.microsoft.com/windows/desktop/api/synchapi/nf-synchapi-waitforsingleobject">WaitForSingleObject</a> function with a wait duration of zero to determine whether a thread has exited. </div>
<div> </div>
<b>Windows Phone 8.1:</b> This function is supported for Windows Phone Store apps on Windows Phone 8.1 and later.

<b>Windows 8.1</b> and <b>Windows Server 2012 R2</b>: This function is supported for Windows Store apps on Windows 8.1, Windows Server 2012 R2, and later.




## -see-also




<a href="https://msdn.microsoft.com/e7f6d054-c535-4521-a3b4-800a9174732f">ExitThread</a>



<a href="https://msdn.microsoft.com/210f7595-ac12-4bb2-bd77-819649ebec10">GetExitCodeProcess</a>



<a href="https://msdn.microsoft.com/d020ecc5-89d1-4a0d-a197-15a66e269e86">OpenThread</a>



<a href="https://msdn.microsoft.com/8c8e8af0-bf50-4a4b-945c-83bae1eff7dd">Process and Thread Functions</a>



<a href="https://msdn.microsoft.com/ae1ad0f3-67df-4573-af22-7086f0470361">TerminateThread</a>



<a href="https://msdn.microsoft.com/633e5d0c-e9d8-4f9a-9411-17cbe9e2e6e4">Terminating a Thread</a>
 

 

