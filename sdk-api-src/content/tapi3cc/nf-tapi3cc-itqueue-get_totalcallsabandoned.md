---
UID: NF:tapi3cc.ITQueue.get_TotalCallsAbandoned
title: ITQueue::get_TotalCallsAbandoned
author: windows-sdk-content
description: The get_TotalCallsAbandoned method gets the number of abandoned calls during the current measurement period.
old-location: tapi3\itqueue_get_totalcallsabandoned.htm
tech.root: tapi
ms.assetid: 2db1309e-f6df-47f8-a695-7bf05d360d99
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITQueue interface [TAPI 2.2],get_TotalCallsAbandoned method, ITQueue.get_TotalCallsAbandoned, ITQueue::get_TotalCallsAbandoned, _tapi3_itqueue_get_totalcallsabandoned, get_TotalCallsAbandoned, get_TotalCallsAbandoned method [TAPI 2.2], get_TotalCallsAbandoned method [TAPI 2.2],ITQueue interface, tapi3.itqueue_get_totalcallsabandoned, tapi3cc/ITQueue::get_TotalCallsAbandoned
ms.topic: method
req.header: tapi3cc.h
req.include-header: Tapi3.h
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
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITQueue.get_TotalCallsAbandoned
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITQueue::get_TotalCallsAbandoned


## -description


The 
<b>get_TotalCallsAbandoned</b> method gets the number of abandoned calls during the current measurement period. The measurement period is switch or implementation specific. (See 
<a href="https://msdn.microsoft.com/931fb7dd-8c9b-4b1e-9296-6335e5a7e164">get_MeasurementPeriod</a>.)


## -parameters




### -param plCalls [out]

Pointer to the number of calls abandoned.


## -returns



This method can return one of these values.

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
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>plCalls</i> is not a valid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TAPI_E_TIMEOUT</b></dt>
</dl>
</td>
<td width="60%">
The operation failed because the TAPI 3 DLL timed it out. The timeout interval is two minutes.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/dd1bc6c7-4d4e-4f66-ac5a-7004b85ec023">ITQueue</a>
 

 

