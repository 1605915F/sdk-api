---
UID: NF:comsvcs.ITransactionProxy.Promote
title: ITransactionProxy::Promote (comsvcs.h)
author: windows-sdk-content
description: Promotes a non-DTC transaction to a DTC transaction.
old-location: cos\itransactionproxy_promote.htm
tech.root: cossdk
ms.assetid: 861103b4-b5fa-4543-b26b-ad0c89d4473d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITransactionProxy interface [COM+],Promote method, ITransactionProxy.Promote, ITransactionProxy::Promote, Promote, Promote method [COM+], Promote method [COM+],ITransactionProxy interface, comsvcs/ITransactionProxy::Promote, cos.itransactionproxy_promote
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
 - ITransactionProxy.Promote
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITransactionProxy::Promote


## -description


Promotes a non-DTC transaction to a DTC transaction.


## -parameters




### -param pTransaction [out]

An implementation of <b>ITransaction</b> that represents the DTC transaction.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, E_UNEXPECTED, and S_OK.




## -remarks



Reasons for promoting a non-DTC transaction to a DTC transaction include exporting the transaction and working with a Queued Moniker Recorder.





## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/comsvcs/nn-comsvcs-itransactionproxy">ITransactionProxy</a>
 

 

