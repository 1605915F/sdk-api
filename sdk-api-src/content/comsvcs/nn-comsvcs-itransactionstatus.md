---
UID: NN:comsvcs.ITransactionStatus
title: ITransactionStatus (comsvcs.h)
author: windows-sdk-content
description: Used to discover the status of the transaction that is completed by the call to CoLeaveServiceDomain when CServiceConfig is configured to use transactions in the call to CoEnterServiceDomain.
old-location: cos\itransactionstatus.htm
tech.root: cossdk
ms.assetid: df5eba93-6db7-478c-b6d7-831c20398d66
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITransactionStatus, ITransactionStatus interface [COM+], ITransactionStatus interface [COM+],described, _cos_ITransactionStatus, comsvcs/ITransactionStatus, cos.itransactionstatus
ms.topic: interface
req.header: comsvcs.h
req.include-header: 
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
 - ITransactionStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITransactionStatus interface


## -description


Used to discover the status of the transaction that is completed by the call to <a href="https://msdn.microsoft.com/b67b3cf6-4462-4578-b61b-c5c61d809822">CoLeaveServiceDomain</a> when <a href="https://msdn.microsoft.com/f546ded4-255e-4565-b588-f36175902778">CServiceConfig</a> is configured to use transactions in the call to <a href="https://msdn.microsoft.com/84640b3b-1f43-4bec-abf6-c295cfb3da8b">CoEnterServiceDomain</a>.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ITransactionStatus</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>ITransactionStatus</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ITransactionStatus</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c8c37aee-c5d2-479f-989f-461877ee6136">GetTransactionStatus</a>
</td>
<td align="left" width="63%">
Retrieves the transaction status.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/0e69758a-8dc7-489c-8e78-ba35749beb01">SetTransactionStatus</a>
</td>
<td align="left" width="63%">
Sets the transaction status to either committed or aborted. Do not use this method. It is used only internally by COM+.


</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/40eccce1-a362-4adc-8060-f6923b9162c9">COM+ Transactions</a>



<a href="https://msdn.microsoft.com/f546ded4-255e-4565-b588-f36175902778">CServiceConfig</a>



<a href="https://msdn.microsoft.com/b67b3cf6-4462-4578-b61b-c5c61d809822">CoLeaveServiceDomain</a>
 

 

