---
UID: NF:wsdhost.IWSDDeviceHost.RegisterPortType
title: IWSDDeviceHost::RegisterPortType (wsdhost.h)
author: windows-sdk-content
description: Registers a port type for incoming messages.
old-location: ncd\iwsddevicehost_registerporttype_method.htm
tech.root: WsdApi
ms.assetid: d514babb-c502-4d9a-b6c8-f371465cb9e8
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWSDDeviceHost interface,RegisterPortType method, IWSDDeviceHost.RegisterPortType, IWSDDeviceHost::RegisterPortType, RegisterPortType, RegisterPortType method, RegisterPortType method,IWSDDeviceHost interface, ncd.iwsddevicehost_registerporttype_method, wsdhost/IWSDDeviceHost::RegisterPortType
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
 - IWSDDeviceHost.RegisterPortType
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWSDDeviceHost::RegisterPortType


## -description


Registers a port type for incoming messages.  All port types listed in the service host metadata must be registered.


## -parameters




### -param pPortType [in]

Reference to a <a href="https://msdn.microsoft.com/ec321771-b3d1-4e7b-b870-009db7c49c6e">WSD_PORT_TYPE</a> structure that describes the port type. 



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
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory to complete the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The port type specified by   <i>pPortType</i> has already been registered.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/497d0331-c88d-4381-8990-94227a9b9659">IWSDDeviceHost</a>
 

 

