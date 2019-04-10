---
UID: NF:threadpoolapiset.IsThreadpoolTimerSet
title: IsThreadpoolTimerSet function (threadpoolapiset.h)
author: windows-sdk-content
description: Determines whether the specified timer object is currently set.
old-location: base\isthreadpooltimerset.htm
tech.root: ProcThread
ms.assetid: f9dee0aa-6310-4218-b207-72a24c5019e2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IsThreadpoolTimerSet, IsThreadpoolTimerSet function, base.isthreadpooltimerset, threadpoolapiset/IsThreadpoolTimerSet, winbase/IsThreadpoolTimerSet
ms.topic: function
req.header: threadpoolapiset.h
req.include-header: Windows 7, Windows Server 2008  Windows Server 2008 R2, Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
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
 - API-MS-Win-Core-threadpool-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-Core-threadpool-l1-2-0.dll
 - API-MS-Win-DownLevel-Kernel32-l1-1-0.dll
 - MinKernelBase.dll
api_name:
 - IsThreadpoolTimerSet
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IsThreadpoolTimerSet function


## -description


Determines whether the specified timer object is currently set.


## -parameters




### -param pti [in, out]

A <b>TP_TIMER</b> structure that defines the timer object. The <a href="https://msdn.microsoft.com/1fa98b79-e646-4e48-9979-1817d2c1b713">CreateThreadpoolTimer</a> function returns this structure.


## -returns



The return value is TRUE if the timer is set; otherwise, the return value is FALSE.




## -remarks



To compile an application that uses this function, define _WIN32_WINNT as 0x0600 or higher.




## -see-also




<a href="https://msdn.microsoft.com/c1270c5d-a1f5-4481-a343-c1ff3301a56e">CloseThreadpoolTimer</a>



<a href="https://msdn.microsoft.com/1fa98b79-e646-4e48-9979-1817d2c1b713">CreateThreadpoolTimer</a>



<a href="https://msdn.microsoft.com/017f88c6-e14c-47ba-94d2-e7bb0dc95d12">SetThreadpoolTimer</a>



<a href="https://msdn.microsoft.com/abe0798a-0b60-4bdb-a61e-45393f1e958d">Thread Pools</a>



<a href="https://msdn.microsoft.com/511488b8-9e92-47b9-8b3c-7ece9d9f996c">WaitForThreadpoolTimerCallbacks</a>
 

 

