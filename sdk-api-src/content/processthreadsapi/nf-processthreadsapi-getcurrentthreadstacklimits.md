---
UID: NF:processthreadsapi.GetCurrentThreadStackLimits
title: GetCurrentThreadStackLimits function (processthreadsapi.h)
author: windows-sdk-content
description: Retrieves the boundaries of the stack that was allocated by the system for the current thread.
old-location: base\getcurrentthreadstacklimits.htm
tech.root: ProcThread
ms.assetid: a5556124-a832-477d-80ab-424779eb9553
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetCurrentThreadStackLimits, GetCurrentThreadStackLimits function, base.getcurrentthreadstacklimits, processthreadsapi/GetCurrentThreadStackLimits
ms.topic: function
f1_keywords: 
 - "processthreadsapi/GetCurrentThreadStackLimits"
req.header: processthreadsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
 - API-MS-Win-Core-ProcessThreads-l1-1-1.dll
 - KernelBase.dll
 - MinKernelBase.dll
 - API-MS-Win-Core-ProcessThreads-l1-1-2.dll
 - API-MS-Win-Core-ProcessThreads-L1-1-3.dll
api_name:
 - GetCurrentThreadStackLimits
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetCurrentThreadStackLimits function


## -description


Retrieves the boundaries of the stack that was allocated by the system for the current thread.


## -parameters




### -param LowLimit [out]

A pointer variable that receives the lower boundary of the current thread stack.


### -param HighLimit [out]

A pointer variable that receives the upper boundary of the current thread stack.


## -returns



This function does not return a value.




## -remarks



    It is possible for user-mode code to execute in stack memory
         that is outside the region allocated by the system when the thread was created. Callers
         can use the <b>GetCurrentThreadStackLimits</b> function to verify that the current stack pointer is within the returned
         limits.


To compile an application that uses this function, set _WIN32_WINNT &gt;= 0x0602. For more information, see <a href="https://docs.microsoft.com/windows/desktop/WinProg/using-the-windows-headers">Using the Windows Headers</a>. 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/ProcThread/thread-stack-size">Thread Stack Size</a>
 

 

