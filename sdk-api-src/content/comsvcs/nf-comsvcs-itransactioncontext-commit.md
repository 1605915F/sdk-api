---
UID: NF:comsvcs.ITransactionContext.Commit
title: ITransactionContext::Commit (comsvcs.h)
author: windows-sdk-content
description: Attempts to commit the work of all COM objects participating in the current transaction. The transaction ends on return from this method.
old-location: cos\itransactioncontext_commit.htm
tech.root: cossdk
ms.assetid: 3945fdf1-6361-413e-9621-18871ded47a4
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Commit, Commit method [COM+], Commit method [COM+],ITransactionContext interface, ITransactionContext interface [COM+],Commit method, ITransactionContext.Commit, ITransactionContext::Commit, _cos_ITransactionContext_Commit, comsvcs/ITransactionContext::Commit, cos.itransactioncontext_commit
ms.topic: method
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - COM
api_location:
 - ComSvcs.h
api_name:
 - ITransactionContext.Commit
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITransactionContext::Commit


## -description


Attempts to commit the work of all COM objects participating in the current transaction. The transaction ends on return from this method.


## -parameters






## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, and E_UNEXPECTED, as well as the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The transaction was committed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The <a href="https://msdn.microsoft.com/efaf1468-4973-472f-af91-85957a52b7df">TransactionContext</a> object is not running under a COM+ process, possibly indicating a corrupted registry entry for the <b>TransactionContext</b> component.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>CONTEXT_E_ABORTED</b></dt>
</dl>
</td>
<td width="60%">
The transaction was aborted.

</td>
</tr>
</table>
 




## -remarks



Calling <b>Commit</b> attempts to commit a transaction. However, the transaction aborts under the following conditions:

<ul>
<li>If a participating object returns from a method after calling <a href="https://msdn.microsoft.com/c254305f-1fc5-417e-b93b-d5e2b36e9e39">SetAbort</a>.</li>
<li>If an object calls <a href="https://msdn.microsoft.com/e83d1223-9b8e-4a92-b98d-9d2b6ed34721">DisableCommit</a> and returns without calling <a href="https://msdn.microsoft.com/6571aadc-bf5a-48c3-817a-66ce444ef96a">EnableCommit</a> or <a href="https://msdn.microsoft.com/8ff25b68-fcb3-4e11-9c74-b49b31806796">SetComplete</a>. 
</li>
<li>If an error causes the Microsoft Distributed Transaction Coordinator (DTC) to abort.
</li>
</ul>
When the method returns, whether the transaction commits or aborts, the transaction ends.




## -see-also




<a href="https://msdn.microsoft.com/818fe18b-04ed-4f54-aeb7-b19aafc8a51a">ITransactionContext</a>
 

 

