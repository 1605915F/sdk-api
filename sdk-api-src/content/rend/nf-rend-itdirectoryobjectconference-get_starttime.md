---
UID: NF:rend.ITDirectoryObjectConference.get_StartTime
title: ITDirectoryObjectConference::get_StartTime (rend.h)
author: windows-sdk-content
description: The get_StartTime method gets the start time of the conference.
old-location: tapi3\itdirectoryobjectconference_get_starttime.htm
tech.root: Tapi
ms.assetid: aeb496d5-2cea-4c69-ba19-c9083d133c1e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ITDirectoryObjectConference interface [TAPI 2.2],get_StartTime method, ITDirectoryObjectConference.get_StartTime, ITDirectoryObjectConference::get_StartTime, _tapi3_itdirectoryobjectconference_get_starttime, get_StartTime, get_StartTime method [TAPI 2.2], get_StartTime method [TAPI 2.2],ITDirectoryObjectConference interface, rend/ITDirectoryObjectConference::get_StartTime, tapi3.itdirectoryobjectconference_get_starttime
ms.topic: method
req.header: rend.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Rend.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Rend.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Rend.dll
api_name:
 - ITDirectoryObjectConference.get_StartTime
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ITDirectoryObjectConference::get_StartTime


## -description


<p class="CCE_Message">[Rendezvous IP Telephony Conferencing controls and interfaces are not available for use in Windows Vista, Windows Server 2008, and subsequent versions of the operating system. The RTC Client API
provides similar functionality.]

The 
<b>get_StartTime</b> method gets the start time of the conference.


## -parameters




### -param pDate [out]

Pointer to the conference start time.


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
The <i>pDate</i> parameter is not a valid pointer.

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
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
Unspecified error.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
This method is not yet implemented.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/bab167cf-2726-4423-87b3-69227404bddc">ITDirectoryObjectConference</a>



<a href="https://msdn.microsoft.com/87ccf59c-3fe6-4247-b7f9-d1fb8bcf4b69">ITDirectoryObjectConference::put_StartTime</a>
 

 

