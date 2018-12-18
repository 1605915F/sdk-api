---
UID: NF:fwpmu.FwpmNetEventEnum3
title: FwpmNetEventEnum3 function
author: windows-sdk-content
description: Returns the next page of results from the network event enumerator.
old-location: fwp\fwpmneteventenum3.htm
tech.root: fwp
ms.assetid: D7098530-9B20-4DB0-908D-EC8E365CB70D
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FwpmNetEventEnum3, FwpmNetEventEnum3 function [Filtering], fwp.fwpmneteventenum3, fwpmu/FwpmNetEventEnum3
ms.topic: function
req.header: fwpmu.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1607 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Fwpuclnt.lib
req.dll: Fwpuclnt.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Fwpuclnt.dll
api_name:
 - FwpmNetEventEnum3
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FwpmNetEventEnum3 function


## -description


The <b>FwpmNetEventEnum3</b> function returns the next page of results from the network event enumerator.
<div class="alert"><b>Note</b>  <b>FwpmNetEventEnum3</b>  s the specific implementation of <b>FwpmNetEventEnum</b> used in Windows 10, version 1607 and later. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 8,  <a href="https://msdn.microsoft.com/bf0974b1-8ddf-4f88-8b15-75f255f7a9d6">FwpmNetEventEnum2</a> is available. For Windows 7, <a href="https://msdn.microsoft.com/b320ab18-2713-479c-a635-da3c5a3e1d10">FwpmNetEventEnum1</a> is available. For Windows Vista, <a href="https://msdn.microsoft.com/c58a273a-c707-47f5-a667-e5d61579d82c">FwpmNetEventEnum0</a> is available.</div><div> </div>

## -parameters




### -param engineHandle [in]

Handle for an open session to the filter engine. Call <a href="https://msdn.microsoft.com/5165f219-f3e0-4e84-915b-75912aab02b7">FwpmEngineOpen0</a> to open a session to the filter engine.


### -param enumHandle [in]

Handle for a network event enumeration created by a call to <a href="https://msdn.microsoft.com/82e0f189-f283-43b2-b9d4-29e754c5c95e">FwpmNetEventCreateEnumHandle0</a>.


### -param numEntriesRequested [in]

The number of enumeration entries requested.


### -param entries [out]

Addresses of enumeration entries.


### -param numEntriesReturned [out]

The number of enumeration entries returned.


## -returns



<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The network events were enumerated successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>FWP_E_NET_EVENTS_DISABLED</b></dt>
<dt>0x80320013</dt>
</dl>
</td>
<td width="60%">
The collection of network diagnostic events is disabled.
Call <a href="https://msdn.microsoft.com/6044a334-a1dc-4447-8581-cd0ffc5883db">FwpmEngineSetOption0</a> to enable it.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>FWP_E_* error code</b></dt>
<dt>0x80320001—0x80320039</dt>
</dl>
</td>
<td width="60%">
A Windows Filtering Platform (WFP) specific error. See <a href="https://msdn.microsoft.com/11f3085a-f044-4a78-b47a-59b9086562bf">WFP Error Codes</a> for details.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_* error code</b></dt>
<dt>0x80010001—0x80010122</dt>
</dl>
</td>
<td width="60%">
Failure to communicate with the remote or local firewall engine.

</td>
</tr>
</table>
 




## -remarks



If the <i>numEntriesReturned</i> is less than the <i>numEntriesRequested</i>, the enumeration is exhausted.

The returned array of entries (but not the individual entries themselves) must be freed by a call to <a href="https://msdn.microsoft.com/ba9f8c1e-f75c-4bf0-b68b-e21a358575fc">FwpmFreeMemory0</a>.

A subsequent call  that uses  the same <i>enumHandle</i> parameter will return the next set of events following those in the  current <i>entries</i> buffer.

<b>FwpmNetEventEnum3</b> returns only events that were logged prior to the creation of the  <i>enumHandle</i> parameter. See <a href="https://msdn.microsoft.com/607b7664-6be4-4ae6-991b-58ac9175405a">Logging</a> for more information.




## -see-also




<a href="https://msdn.microsoft.com/2D71C44C-B553-46DD-8943-DCC979A7DC6B">FWPM_NET_EVENT3</a>



<a href="https://msdn.microsoft.com/82e0f189-f283-43b2-b9d4-29e754c5c95e">FwpmNetEventCreateEnumHandle0</a>



<a href="https://msdn.microsoft.com/607b7664-6be4-4ae6-991b-58ac9175405a">WFP Logging</a>
 

 

