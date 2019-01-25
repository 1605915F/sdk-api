---
UID: NF:tapi3cc.ITQueue.get_AverageWaitTime
title: ITQueue::get_AverageWaitTime
author: windows-sdk-content
description: The get_AverageWaitTime method gets the average time in the queue (in seconds) for a call during the current measurement period.
old-location: tapi3\itqueue_get_averagewaittime.htm
tech.root: Tapi
ms.assetid: 94883656-8a72-464d-9478-89f698c98db8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITQueue interface [TAPI 2.2],get_AverageWaitTime method, ITQueue.get_AverageWaitTime, ITQueue::get_AverageWaitTime, _tapi3_itqueue_get_averagewaittime, get_AverageWaitTime, get_AverageWaitTime method [TAPI 2.2], get_AverageWaitTime method [TAPI 2.2],ITQueue interface, tapi3.itqueue_get_averagewaittime, tapi3cc/ITQueue::get_AverageWaitTime
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
 - ITQueue.get_AverageWaitTime
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITQueue::get_AverageWaitTime


## -description


The 
<b>get_AverageWaitTime</b> method gets the average time in the queue (in seconds) for a call during the current measurement period. The measurement period is switch or implementation specific. (See 
<a href="https://msdn.microsoft.com/931fb7dd-8c9b-4b1e-9296-6335e5a7e164">get_MeasurementPeriod</a>.)


## -parameters




### -param plWaitTime [out]

Pointer to the average wait time.


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
The <i>plWaitTime</i> is not a valid pointer.

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
 

 

