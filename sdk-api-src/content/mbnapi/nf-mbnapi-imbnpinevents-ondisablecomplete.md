---
UID: NF:mbnapi.IMbnPinEvents.OnDisableComplete
title: IMbnPinEvents::OnDisableComplete
author: windows-sdk-content
description: Notification method called by the Mobile Broadband service to indicate that a PIN disable operation has completed.
old-location: mbn\imbnpinevents_ondisablecomplete.htm
tech.root: mbn
ms.assetid: 54fc0ec1-eb35-4403-b22a-4c50c4912604
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: E_FAIL, E_MBN_BAD_SIM, E_MBN_FAILURE, E_MBN_PIN_REQUIRED, E_MBN_SIM_NOT_INSERTED, HRESULT_FROM_WIN32(ERROR_NOT_SUPPORTED), IMbnPinEvents interface [Microsoft Broadband Networks],OnDisableComplete method, IMbnPinEvents.OnDisableComplete, IMbnPinEvents::OnDisableComplete, OnDisableComplete, OnDisableComplete method [Microsoft Broadband Networks], OnDisableComplete method [Microsoft Broadband Networks],IMbnPinEvents interface, S_OK, mbn.imbnpinevents_ondisablecomplete, mbnapi/IMbnPinEvents::OnDisableComplete
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mbnapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mbnapi.idl
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
 - mbnapi.h
api_name:
 - IMbnPinEvents.OnDisableComplete
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMbnPinEvents::OnDisableComplete


## -description


Notification method called by the Mobile Broadband service to indicate that a PIN disable operation has completed.


## -parameters




### -param pin [in]

An <a href="https://msdn.microsoft.com/76764dbb-7de0-4b95-a210-60b8e6a4b24b">IMbnPin</a> interface that the PIN type.


### -param pinInfo [in]

A pointer to a <a href="https://msdn.microsoft.com/c70b45ea-c16b-4d0d-946a-f543c827c458">MBN_PIN_INFO</a> structure that contains information on remaining attempts, in case of failure operations.  The contents of <i>pinInfo</i> are meaningful only when <i>status</i> is <b>E_MBN_FAILURE</b>.  


### -param requestID [in]

A request ID set by the Mobile Broadband service to identify the PIN disable request.


### -param status [in]

A status code that indicates the outcome of the operation.

A calling application can expect one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="S_OK"></a><a id="s_ok"></a><dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The operation was  successful.

</td>
</tr>
<tr>
<td width="40%"><a id="HRESULT_FROM_WIN32_ERROR_NOT_SUPPORTED_"></a><a id="hresult_from_win32_error_not_supported_"></a><dl>
<dt><b>HRESULT_FROM_WIN32(ERROR_NOT_SUPPORTED)</b></dt>
</dl>
</td>
<td width="60%">
The device does not support this operation.

</td>
</tr>
<tr>
<td width="40%"><a id="E_FAIL"></a><a id="e_fail"></a><dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The operation could not be completed.

</td>
</tr>
<tr>
<td width="40%"><a id="E_MBN_PIN_REQUIRED"></a><a id="e_mbn_pin_required"></a><dl>
<dt><b>E_MBN_PIN_REQUIRED</b></dt>
</dl>
</td>
<td width="60%">
A PIN is required for the operation to complete.  The calling application can call the <a href="https://msdn.microsoft.com/34378403-cf58-4ada-9eb6-f5dad5f69bc9">GetPinState</a> method of <a href="https://msdn.microsoft.com/b5cfabc7-81f8-4ea0-b6f4-5de011320f0b">IMbnPinManager</a> to discover the type of expected PIN.

</td>
</tr>
<tr>
<td width="40%"><a id="E_MBN_SIM_NOT_INSERTED"></a><a id="e_mbn_sim_not_inserted"></a><dl>
<dt><b>E_MBN_SIM_NOT_INSERTED</b></dt>
</dl>
</td>
<td width="60%">
There is no SIM in the device.

</td>
</tr>
<tr>
<td width="40%"><a id="E_MBN_BAD_SIM"></a><a id="e_mbn_bad_sim"></a><dl>
<dt><b>E_MBN_BAD_SIM</b></dt>
</dl>
</td>
<td width="60%">
There is a bad SIM in the device.

</td>
</tr>
<tr>
<td width="40%"><a id="E_MBN_FAILURE"></a><a id="e_mbn_failure"></a><dl>
<dt><b>E_MBN_FAILURE</b></dt>
</dl>
</td>
<td width="60%">
There is a failed attempt to use the PIN.

</td>
</tr>
</table>
 


## -returns



This method must return <b>S_OK</b>.




## -remarks



The <b>OnDisableComplete</b> method is called by the Mobile Broadband service to report the completion status of a PIN disable operation initialized by a call to the <a href="https://msdn.microsoft.com/612edeb9-3de4-48ac-a311-7238402e8658">Disable</a> method of <a href="https://msdn.microsoft.com/76764dbb-7de0-4b95-a210-60b8e6a4b24b">IMbnPin</a>.

The contents of <i>pinInfo</i> are meaningful only when <i>status</i> is <b>E_MBN_FAILURE</b>.  The <b>pinState</b> member should be ignored and <b>pinType</b> field is set to the PIN type of the current <a href="https://msdn.microsoft.com/76764dbb-7de0-4b95-a210-60b8e6a4b24b">IMbnPin</a> interface. This structure contains the attempts remaining to enter a valid PIN. 


For example, if the PIN passed to change a PIN type is incorrect then the operation will fail with a status code of <b>E_MBN_FAILURE</b>. In this case, <b>pinInfo.attemptsRemaining</b> specifies the number of attempts remaining to retry this operation.
If repeated attempts with the wrong PIN causes <b>attemptsRemaining</b> to become 0 then the application can call the <a href="https://msdn.microsoft.com/34378403-cf58-4ada-9eb6-f5dad5f69bc9">GetPinState</a> method of  <a href="https://msdn.microsoft.com/b5cfabc7-81f8-4ea0-b6f4-5de011320f0b">IMbnPinManager</a> to get the type of PIN required.




## -see-also




<a href="https://msdn.microsoft.com/4bdaa4e5-880e-4d1f-aec1-36811a0f21c1">IMbnPinEvents</a>
 

 

