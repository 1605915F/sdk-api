---
UID: NF:portabledeviceapi.IPortableDeviceCapabilities.GetSupportedCommands
title: IPortableDeviceCapabilities::GetSupportedCommands (portabledeviceapi.h)
author: windows-sdk-content
description: The GetSupportedCommands method retrieves a list of all the supported commands for this device.
old-location: wpdsdk\iportabledevicecapabilities_getsupportedcommands.htm
tech.root: wpd_sdk
ms.assetid: 974b16c7-27a0-40a6-8941-e93293a69b48
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSupportedCommands, GetSupportedCommands method [Windows Portable Devices SDK], GetSupportedCommands method [Windows Portable Devices SDK],IPortableDeviceCapabilities interface, IPortableDeviceCapabilities interface [Windows Portable Devices SDK],GetSupportedCommands method, IPortableDeviceCapabilities.GetSupportedCommands, IPortableDeviceCapabilities::GetSupportedCommands, IPortableDeviceCapabilitiesGetSupportedCommands, portabledeviceapi/IPortableDeviceCapabilities::GetSupportedCommands, wpdsdk.iportabledevicecapabilities_getsupportedcommands
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
 - IPortableDeviceCapabilities.GetSupportedCommands
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPortableDeviceCapabilities::GetSupportedCommands


## -description


The <b>GetSupportedCommands</b> method retrieves a list of all the supported commands for this device.
      


## -parameters




### -param ppCommands [out]

Address of a variable that receives a pointer to an <a href="https://msdn.microsoft.com/2460f5bc-6b1c-4e3b-bdb9-faaa6d6c87fd">IPortableDeviceKeyCollection</a> interface that holds all the valid commands. For a list of commands that are defined by Windows Portable Devices, see <a href="https://msdn.microsoft.com/f579745a-5327-4c8b-bfa7-fe81d9657a3b">Commands</a>. The caller must release this interface when it is done with it.
          


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
</table>
 




## -remarks



None.
      




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd319362(v=VS.85).aspx">IPortableDeviceCapabilities Interface</a>
 

 

