---
UID: NF:tapi3if.ITAddressDeviceSpecificEvent.get_Call
title: ITAddressDeviceSpecificEvent::get_Call (tapi3if.h)
author: windows-sdk-content
description: The get_Call method gets a pointer to the ITCallInfo interface pointer for the call object involved in the event.
old-location: tapi3\itaddressdevicespecificevent_get_call.htm
tech.root: Tapi
ms.assetid: dcf3b82d-5c1f-41f7-bb6a-6470a96f4049
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITAddressDeviceSpecificEvent interface [TAPI 2.2],get_Call method, ITAddressDeviceSpecificEvent.get_Call, ITAddressDeviceSpecificEvent::get_Call, _tapi3_itaddressdevicespecificevent_get_call, get_Call, get_Call method [TAPI 2.2], get_Call method [TAPI 2.2],ITAddressDeviceSpecificEvent interface, tapi3.itaddressdevicespecificevent_get_call, tapi3if/ITAddressDeviceSpecificEvent::get_Call
ms.topic: method
req.header: tapi3if.h
req.include-header: 
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
 - ITAddressDeviceSpecificEvent.get_Call
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITAddressDeviceSpecificEvent::get_Call


## -description


The 
<b>get_Call</b> method gets a pointer to the 
<a href="https://msdn.microsoft.com/5209d4a1-e05b-453e-8896-2dc71f0b9af0">ITCallInfo</a> interface pointer for the call object involved in the event.


## -parameters




### -param ppCall [out]

Pointer to the 
<a href="https://msdn.microsoft.com/5209d4a1-e05b-453e-8896-2dc71f0b9af0">ITCallInfo</a> interface.


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
The <i>ppCall</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/8590e9b1-2bbf-47e5-96de-8765a475a972">ITAddressDeviceSpecificEvent</a>



<a href="https://msdn.microsoft.com/5209d4a1-e05b-453e-8896-2dc71f0b9af0">ITCallInfo</a>
 

 

