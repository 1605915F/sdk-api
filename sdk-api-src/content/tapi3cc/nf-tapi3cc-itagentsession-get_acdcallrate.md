---
UID: NF:tapi3cc.ITAgentSession.get_ACDCallRate
title: ITAgentSession::get_ACDCallRate (tapi3cc.h)
author: windows-sdk-content
description: The get_ACDCallRate method gets the all rate per agent session, in calls per hour.
old-location: tapi3\itagentsession_get_acdcallrate.htm
tech.root: Tapi
ms.assetid: 49737945-7e27-4c88-94c5-29db7dccfc97
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITAgentSession interface [TAPI 2.2],get_ACDCallRate method, ITAgentSession.get_ACDCallRate, ITAgentSession::get_ACDCallRate, _tapi3_itagentsession_get_acdcallrate, get_ACDCallRate, get_ACDCallRate method [TAPI 2.2], get_ACDCallRate method [TAPI 2.2],ITAgentSession interface, tapi3.itagentsession_get_acdcallrate, tapi3cc/ITAgentSession::get_ACDCallRate
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
 - ITAgentSession.get_ACDCallRate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITAgentSession::get_ACDCallRate


## -description


The 
<b>get_ACDCallRate</b> method gets the all rate per agent session, in calls per hour.


## -parameters




### -param pcyCallrate [out]

Pointer to call rate.


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
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>pcyCallrate</i> parameter is not a valid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>LINEERR_</b></dt>
</dl>
</td>
<td width="60%">
See 
<a href="https://msdn.microsoft.com/06a5ea23-4205-46fd-abe7-ee4575be81c8">lineGetAgentSessionInfo</a> for error codes returned from this TAPI 2.1 function.

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
 




## -remarks



This method wraps the TAPI 2.1 
<a href="https://msdn.microsoft.com/06a5ea23-4205-46fd-abe7-ee4575be81c8">lineGetAgentSessionInfo</a> function.




## -see-also




<a href="https://msdn.microsoft.com/b0db0834-7b9b-4a72-9cc6-6cba31ed1275">ITAgentSession</a>



<a href="https://msdn.microsoft.com/06a5ea23-4205-46fd-abe7-ee4575be81c8">lineGetAgentSessionInfo</a>
 

 

