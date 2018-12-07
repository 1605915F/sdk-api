---
UID: NF:rpcasync.RpcSsContextLockExclusive
title: RpcSsContextLockExclusive function
author: windows-sdk-content
description: The RpcSsContextLockExclusive function enables an application to begin using a context handle in exclusive mode.
old-location: rpc\rpcsscontextlockexclusive.htm
tech.root: rpc
ms.assetid: 7ef2376b-da25-4e4b-8a25-0913d680945f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: RpcSsContextLockExclusive, RpcSsContextLockExclusive function [RPC], _rpc_rpcsscontextlockexclusive, rpc.rpcsscontextlockexclusive, rpcasync/RpcSsContextLockExclusive
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: rpcasync.h
req.include-header: Rpc.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Rpcrt4.lib
req.dll: Rpcrt4.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Rpcrt4.dll
api_name:
 - RpcSsContextLockExclusive
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# RpcSsContextLockExclusive function


## -description


The 
<b>RpcSsContextLockExclusive</b> function enables an application to begin using a context handle in exclusive mode. The 
<b>RpcSsContextLockExclusive</b> function enables methods declared as nonserialized (shared) in the IDL or ACF file to be dynamically changed to access a context handle in serialized (exclusive) mode.


## -parameters




### -param ServerBindingHandle [in]

Binding handle on the server that represents a binding to a client. The server impersonates the client indicated by this handle. If a value of zero is specified, the server impersonates the client that is being served by this server thread.


### -param UserContext [in]

Pointer passed to the manager or server routine by RPC. See Remarks. 




For out-only context handles, the 
<b>RpcSsContextLockExclusive</b> function performs no operation.


## -returns



Returns RPC_S_OK upon successful execution, indicating the thread now has access to the context handle in exclusive mode. Returns ERROR_MORE_WRITES when multiple threads attempt an exclusive lock on the context handle. See Remarks.

<div class="alert"><b>Note</b>  For a list of valid error codes, see 
<a href="https://msdn.microsoft.com/0223aa7a-b0cf-49e3-9f08-90be5ccffbd1">RPC Return Values</a>.</div>
<div> </div>



## -remarks



Modifying whether a context handle is serialized or nonserialized can be useful to applications that determine whether to close a context handle based on conditions detected upon execution. To change a context handle from serialized (exclusive) to nonserialized (shared), use the 
<a href="https://msdn.microsoft.com/469f0995-54ff-40a6-9322-3d173e2c9861">RpcSsContextLockShared</a> function.

For the <i>UserContext</i> parameter, if the manager routine receives a pointer to a context handle, it must pass the 
<b>RpcSsContextLockExclusive</b> function the same pointer it received from RPC. If the manager routine receives the context handle itself, which is typical for [in] only context handles, it must pass the context handle itself to the 
<b>RpcSsContextLockExclusive</b> function. The following code example demonstrates this:

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>void _UseShared(
    /* [in] */ handle_t Binding,
    //...
    /* [in] */ TestContextHandleShared *Ctx,
    //...
    )
{
    //...
    RpcStatus = RpcSsContextLockExclusive(Binding, Ctx);
    //...
}
</pre>
</td>
</tr>
</table></span></div>
If a manager routine takes multiple [in, out] context handles as an argument, RPC gives the manager routine a pointer to the context handle, not the context handle itself. The pointer is guaranteed to be unique, and therefore passing it to the 
<b>RpcSsContextLockExclusive</b> function is unambiguous. However, if a function takes multiple [in] only context handles, RPC gives the manager routine the context handle itself. Therefore, the context handle may not be unique. In this case, RPC executes this function on the first context handle with the given value.

Methods should not modify a context handle when in shared mode. Calling the 
<b>RpcSsContextLockExclusive</b> function does not eliminate a reader lock on the specified context handle; this ensures an unchanged context handle for applications that do not modify context handles in shared mode. If two threads attempt to obtain an exclusive lock on the same context handle by calling the 
<b>RpcSsContextLockExclusive</b> function at the same time, one arbitrarily chosen thread is returned RPC_S_OK, and the other is returned ERROR_MORE_WRITES. The thread that is returned ERROR_MORE_WRITES receives an exclusive lock, but its reader lock on the context handle is lost upon return. A caller receiving ERROR_MORE_WRITES must assume nothing about the context handle upon return of the 
<b>RpcSsContextLockExclusive</b> function, as it may have been destroyed.

Asynchronous calls must not use the 
<b>RpcSsContextLockExclusive</b> function on the same call object from more than one thread at a time.

The 
<b>RpcSsContextLockExclusive</b> function can fail due to out-of-memory conditions, and RPC servers must therefore be prepared to handle such errors.




## -see-also




<a href="https://msdn.microsoft.com/469f0995-54ff-40a6-9322-3d173e2c9861">RpcSsContextLockShared</a>



<a href="https://msdn.microsoft.com/">context_handle</a>



<a href="https://msdn.microsoft.com/aff2484e-639b-41d2-94a9-f34ca4f2343c">context_handle_noserialize</a>



<a href="https://msdn.microsoft.com/e2f48582-228a-4725-9543-1e638d86ff6b">context_handle_serialize</a>
 

 

