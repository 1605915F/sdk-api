---
UID: NF:tapi3cc.ITAgent.get_NumberOfACDCalls
title: ITAgent::get_NumberOfACDCalls
author: windows-sdk-content
description: The get_NumberOfACDCalls method gets the number of ACD calls handled by this agent across all sessions.
old-location: tapi3\itagent_get_numberofacdcalls.htm
tech.root: Tapi
ms.assetid: bef36468-8ee9-4ce2-bf8d-e2bd8c986ae3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITAgent interface [TAPI 2.2],get_NumberOfACDCalls method, ITAgent.get_NumberOfACDCalls, ITAgent::get_NumberOfACDCalls, _tapi3_itagent_get_numberofacdcalls, get_NumberOfACDCalls, get_NumberOfACDCalls method [TAPI 2.2], get_NumberOfACDCalls method [TAPI 2.2],ITAgent interface, tapi3.itagent_get_numberofacdcalls, tapi3cc/ITAgent::get_NumberOfACDCalls
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
 - ITAgent.get_NumberOfACDCalls
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITAgent::get_NumberOfACDCalls


## -description


The 
<b>get_NumberOfACDCalls</b> method gets the number of ACD calls handled by this agent across all sessions.

The measurement period over which this information is calculated is switch- and/or implementation-specific. (See 
<a href="https://msdn.microsoft.com/ccc91dfb-83e5-496a-921d-784fcaea5af5">get_MeasurementPeriod</a>.)


## -parameters




### -param plCalls [out]

Total number of calls.


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
The <i>plCalls</i> parameter is not a valid pointer.

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




<a href="https://msdn.microsoft.com/6c1409c9-da73-4d21-bf56-07e9ab7b33a0">ITAgent</a>
 

 

