---
UID: NF:webservices.WsAbortChannel
title: WsAbortChannel function
author: windows-sdk-content
description: Cancels all pending I/O for a specified channel.
old-location: wsw\wsabortchannel.htm
tech.root: wsw
ms.assetid: 67af85d7-db75-4e26-a7cc-8115ac3f2d59
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WsAbortChannel, WsAbortChannel function [Web Services for Windows], webservices/WsAbortChannel, wsw.wsabortchannel
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: webservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WebServices.lib
req.dll: WebServices.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - WebServices.dll
api_name:
 - WsAbortChannel
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WsAbortChannel function


## -description



Cancels all pending I/O for  a specified channel




## -parameters




### -param channel [in]

A   pointer to a <a href="https://msdn.microsoft.com/741636a4-5e0f-495a-bb1d-1a00cfd6f65a">WS_CHANNEL</a>  structure representing the channel for which 
                    to cancel I/O.
                


### -param error [in, optional]

Pointer to a <a href="https://msdn.microsoft.com/d5763d93-8eff-4df8-9a8a-a58aefabcb21">WS_ERROR</a> structure that receives additional error information if the function fails.
                


## -returns



If the function succeeds, it returns NO_ERROR; otherwise, it returns an HRESULT error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WS_E_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
See the Remarks section for platform limitations.
                

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One or more arguments are invalid.

</td>
</tr>
</table>
 




## -remarks




<b>Windows Server 2003 and before:  </b>On Windows platforms before Windows Vista, this function is not supported for WS_UDP_CHANNEL_BINDING or WS_HTTP_CHANNEL_BINDING  if the channel is in the WS_CHANNEL_STATE_ACCEPTING state and the listener has not already been aborted. 

(For information on channel bindings and channel states, see the <a href="https://msdn.microsoft.com/554cc239-feab-4262-9821-6478a3d93ffc">WS_CHANNEL_BINDING</a> and <a href="https://msdn.microsoft.com/3a7f5bbd-e484-4a7e-8e5d-df229a7227a5">WS_CHANNEL_STATE</a> enumerations.)<p class="note"> This function is also not supported for WS_HTTP_CHANNEL_BINDING with WS_CHANNEL_TYPE_REPLY when aborting a channel  in the WS_CHANNEL_STATE_OPEN or WS_CHANNEL_STATE_FAULTED state. (For information on channel types, see the <a href="https://msdn.microsoft.com/7e1092f9-10e8-485c-a286-770e1c74d8ca">WS_CHANNEL_TYPE</a> enumeration.





<b>WsAbortChannel</b> can be called for a channel in any state, and does not wait for pending I/O to complete before aborting the channel.
            
                

If the channel is in the   <b>WS_CHANNEL_STATE_OPEN</b> state, <b>WsAbortChannel</b> causes the channel to fault to the <b>WS_CHANNEL_STATE_FAULTED</b> state. <div class="alert"><b>Note</b>  See 
                <a href="https://msdn.microsoft.com/b8f5da50-d296-4550-8810-114d1f0e810b">WsAbandonMessage</a> for information on how to skip a particular
                message and keep the channel open.
            </div>
<div> </div>If called with valid parameters, this function will not fail for reasons such as a lack of system resources. However, note the limitations on some operating systems versions at the beginning of Remarks. 



