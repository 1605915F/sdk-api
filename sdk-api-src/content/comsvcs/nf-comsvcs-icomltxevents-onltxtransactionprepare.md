---
UID: NF:comsvcs.IComLTxEvents.OnLtxTransactionPrepare
title: IComLTxEvents::OnLtxTransactionPrepare
author: windows-sdk-content
description: Generated when COM+ receives a prepare notification for a transaction.
old-location: cos\icomltxevents_onltxtransactionprepare.htm
tech.root: cossdk
ms.assetid: 31915d4c-7ac0-406b-b2d2-ab96b317be3f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComLTxEvents interface [COM+],OnLtxTransactionPrepare method, IComLTxEvents.OnLtxTransactionPrepare, IComLTxEvents::OnLtxTransactionPrepare, OnLtxTransactionPrepare, OnLtxTransactionPrepare method [COM+], OnLtxTransactionPrepare method [COM+],IComLTxEvents interface, comsvcs/IComLTxEvents::OnLtxTransactionPrepare, cos.icomltxevents_onltxtransactionprepare
ms.topic: method
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
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
 - IComLTxEvents.OnLtxTransactionPrepare
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComLTxEvents::OnLtxTransactionPrepare


## -description


Generated when COM+ receives a prepare notification for a transaction.

The event ID for this event is EID_LTXPREPARE.



## -parameters




### -param pInfo [in]

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/ms688276(v=VS.85).aspx">COMSVCSEVENTINFO</a> structure.


### -param guidLtx [in]

A GUID that identifies the transaction.


### -param fVote [in]

The COM+ vote for the prepare request.


## -returns



The user verifies the return values from this method.




## -see-also




<a href="https://msdn.microsoft.com/8be6dddb-ed57-4715-8933-8a0e478095c8">IComLTxEvents</a>
 

 

