---
UID: NF:portabledeviceapi.IPortableDevice.Capabilities
title: IPortableDevice::Capabilities (portabledeviceapi.h)
author: windows-sdk-content
description: The Capabilities method retrieves an interface used to query the capabilities of a portable device.
old-location: wpdsdk\iportabledevice_capabilities.htm
tech.root: wpd_sdk
ms.assetid: 3d44e488-1bef-4cdd-bb0b-2b8154deb19e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Capabilities, Capabilities method [Windows Portable Devices SDK], Capabilities method [Windows Portable Devices SDK],IPortableDevice interface, IPortableDevice interface [Windows Portable Devices SDK],Capabilities method, IPortableDevice.Capabilities, IPortableDevice::Capabilities, IPortableDeviceCapabilities, portabledeviceapi/IPortableDevice::Capabilities, wpdsdk.iportabledevice_capabilities
ms.topic: method
req.header: portabledeviceapi.h
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
req.lib: PortableDeviceGUIDs.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - PortableDeviceGUIDs.lib
 - PortableDeviceGUIDs.dll
api_name:
 - IPortableDevice.Capabilities
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPortableDevice::Capabilities


## -description


The <b>Capabilities</b> method retrieves an interface used to query the capabilities of a portable device.
      


## -parameters




### -param ppCapabilities [out]

Address of a variable that receives a pointer to an <a href="https://msdn.microsoft.com/en-us/library/Dd319362(v=VS.85).aspx">IPortableDeviceCapabilities</a> interface that can describe the device's capabilities. The caller must release this interface when it is done with it.
          


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.
          

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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppCapabilities</i> argument was a <b>NULL</b> pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/98c48e56-56b8-4800-b52b-ac08f2abf27e">IPortableDevice Interface</a>



<a href="https://msdn.microsoft.com/7748e111-9987-4685-8fc8-10c5d4631080">Retrieving the Functional Categories Supported by a Device</a>



<a href="https://msdn.microsoft.com/2332e3cc-087c-49cf-bde9-7f86f65158e7">Retrieving the Rendering Capabilities Supported by a Device</a>
 

 

