---
UID: NF:threadpoolapiset.QueryThreadpoolStackInformation
title: QueryThreadpoolStackInformation function
author: windows-sdk-content
description: Retrieves the stack reserve and commit sizes for threads in the specified thread pool.
old-location: base\querythreadpoolstackinformation.htm
tech.root: procthread
ms.assetid: 1669dfa7-75bf-4776-bba7-7d03a084a32c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: QueryThreadpoolStackInformation, QueryThreadpoolStackInformation function, base.querythreadpoolstackinformation, threadpoolapiset/QueryThreadpoolStackInformation, winbase/QueryThreadpoolStackInformation
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: threadpoolapiset.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - kernel32.dll
 - API-MS-Win-Core-threadpool-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-Core-threadpool-l1-2-0.dll
 - API-MS-Win-DownLevel-Kernel32-l1-1-0.dll
 - MinKernelBase.dll
api_name:
 - QueryThreadpoolStackInformation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# QueryThreadpoolStackInformation function


## -description


Retrieves the stack reserve and commit sizes for threads in the specified thread pool.


## -parameters




### -param ptpp [in]

A <b>TP_POOL</b> structure that specifies the thread pool. The <a href="https://msdn.microsoft.com/cc00d7bf-ac52-44ff-a6a8-76c8eaace5e6">CreateThreadpool</a> function returns this structure.


### -param ptpsi [out]

A <b>TP_POOL_STACK_INFORMATION</b> structure that receives the stack reserve and commit size. 


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. 




## -remarks



To compile an application that uses this function, set _WIN32_WINNT to _WIN32_WINNT_WIN7. For more information, see <a href="https://msdn.microsoft.com/a4def563-8ddc-4630-ae8a-86c07cf98374">Using the Windows Headers</a>.




## -see-also




<a href="https://msdn.microsoft.com/dbed0a95-30d8-4e63-b141-743401103c53">SetThreadpoolStackInformation</a>
 

 

