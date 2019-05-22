---
UID: NF:winnt._InlineInterlockedAdd
title: _InlineInterlockedAdd function (winnt.h)
author: windows-sdk-content
description: Performs an atomic addition operation on the specified LONG values. The operation is performed with acquire memory ordering semantics.
old-location: base\interlockedaddacquire.htm
tech.root: Sync
ms.assetid: ec1746cc-aff9-440e-b7e1-15a3d7a0fa58
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: InterlockedAddAcquire, InterlockedAddAcquire function, _InlineInterlockedAdd, base.interlockedaddacquire, winnt/InterlockedAddAcquire
ms.topic: function
req.header: winnt.h
req.include-header: Windows.h
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
 - Winnt.h
api_name:
 - InterlockedAddAcquire
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# _InlineInterlockedAdd function


## -description


Performs an atomic addition operation on the specified <b>LONG</b> values. The operation is performed with acquire memory ordering semantics.


## -parameters




### -param Addend [in, out]

A pointer to the first operand. This value will be replaced with the result of the operation.


### -param Value [in]

The second operand.


## -returns



The function returns the result of the operation.




## -remarks



The interlocked functions provide a simple mechanism for synchronizing access to a variable that is shared by multiple threads. This function is atomic with respect to calls to other interlocked functions.

This function is implemented using a compiler intrinsic where possible. For more information, see the WinBase.h header file and <a href="https://msdn.microsoft.com/library/51s265a6(v=VS.85).aspx">_InterlockedAdd_acq</a>.

<div class="alert"><b>Note</b>  This function is supported on Windows RT-based systems.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/729c0e68-ef52-4d6c-b771-a89043a937e6">Interlocked Variable Access</a>



<a href="https://msdn.microsoft.com/c3ff4c2f-ac84-4046-ac4e-600569b874be">InterlockedAdd</a>



<a href="https://msdn.microsoft.com/ab37292f-4291-4cca-826c-d6488e141db8">InterlockedAdd64</a>



<a href="https://msdn.microsoft.com/0bdce93f-a57a-40d3-a8fa-007edb8b5c6d">InterlockedAddAcquire64</a>



<a href="https://msdn.microsoft.com/98f29a64-27c9-455f-a7cf-c2c47ea512c8">InterlockedAddNoFence</a>



<a href="https://msdn.microsoft.com/f7c8c50a-805f-4963-8a5e-160776dd995e">InterlockedAddNoFence64</a>



<a href="https://msdn.microsoft.com/d09a6420-bf6c-43a7-aa7a-1cff03596afc">InterlockedAddRelease</a>



<a href="https://msdn.microsoft.com/24a88190-79e3-48bf-986e-d5d08c1bce08">InterlockedAddRelease64</a>



<a href="https://msdn.microsoft.com/en-us/library/ms683597(v=VS.85).aspx">InterlockedExchangeAdd</a>



<a href="https://msdn.microsoft.com/9b6359c2-0113-49b6-83d0-316ad95aba1b">Synchronization Functions</a>
 

 

