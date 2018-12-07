---
UID: NF:wsdhost.IWSDDeviceHost.Stop
title: IWSDDeviceHost::Stop
author: windows-sdk-content
description: Sends a WS-Discovery Bye message and stops the host.
old-location: ncd\iwsddevicehost_stop_method.htm
tech.root: wsdapi
ms.assetid: 7a31e45a-7d38-44b7-84c7-7471bc14cc94
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWSDDeviceHost interface,Stop method, IWSDDeviceHost.Stop, IWSDDeviceHost::Stop, Stop, Stop method, Stop method,IWSDDeviceHost interface, ncd.iwsddevicehost_stop_method, wsdhost/IWSDDeviceHost::Stop
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wsdhost.h
req.include-header: Wsdapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WsdHost.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Wsdapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wsdapi.dll
api_name:
 - IWSDDeviceHost.Stop
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWSDDeviceHost::Stop


## -description


Sends a WS-Discovery <a href="https://msdn.microsoft.com/7b9abfcc-28ab-4f29-af69-6dc68e3f51b6">Bye</a> message and stops the host. After a host has been successfully stopped, it must be terminated with <a href="https://msdn.microsoft.com/2a8df6fb-2834-44f4-9f25-454dcc2ff660">IWSDDeviceHost::Terminate</a> before being released.


## -parameters






## -returns



Possible return values include, but are not limited to, the following:

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
Method completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The host has already stopped.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The host is not initialized or the host is not started.

</td>
</tr>
</table>
 




## -remarks



When a device host is stopped using this method, all services remain attached but no inbound messages are processed or otherwise handled. 

Calling <b>Stop</b> is not necessary if the host has not been started.





## -see-also




<a href="https://msdn.microsoft.com/497d0331-c88d-4381-8990-94227a9b9659">IWSDDeviceHost</a>
 

 

