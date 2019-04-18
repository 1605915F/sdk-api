---
UID: NF:portabledeviceapi.IPortableDeviceContent.Properties
title: IPortableDeviceContent::Properties (portabledeviceapi.h)
author: windows-sdk-content
description: The Properties method retrieves the interface that is required to get or set properties on an object on the device.
old-location: wpdsdk\iportabledevicecontent_properties.htm
tech.root: wpd_sdk
ms.assetid: bc3ba717-1be3-4f29-ac27-6bdcbc5ed94f
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IPortableDeviceContent interface [Windows Portable Devices SDK],Properties method, IPortableDeviceContent.Properties, IPortableDeviceContent::Properties, IPortableDeviceContentProperties, Properties, Properties method [Windows Portable Devices SDK], Properties method [Windows Portable Devices SDK],IPortableDeviceContent interface, portabledeviceapi/IPortableDeviceContent::Properties, wpdsdk.iportabledevicecontent_properties
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
 - IPortableDeviceContent.Properties
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPortableDeviceContent::Properties


## -description


The <b>Properties</b> method retrieves the interface that is required to get or set properties on an object on the device.
      


## -parameters




### -param ppProperties [out]

Address of a variable that receives a pointer to an <a href="https://msdn.microsoft.com/4555e85b-c667-466c-a527-cc29ca7a6aee">IPortableDeviceProperties</a> interface that is used to get or set object properties. The caller must release this interface when it is done with it.
          


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
At least one of the required arguments was a <b>NULL</b> pointer.

</td>
</tr>
</table>
 




## -remarks



The retrieved interface is not specific to a particular object on the device; it is specific only to the device. You must specify the ID of the object you want when requesting or setting properties.
      


#### Examples

For an example of how to use this method, see <a href="https://msdn.microsoft.com/1c003534-96b4-419b-94d1-73b5ffa2eba1">Setting Properties for a Single Object</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd388529(v=VS.85).aspx">IPortableDeviceContent Interface</a>



<a href="https://msdn.microsoft.com/7fbd6f65-366a-49ea-a680-be77ca0d64f2">Retrieving Content-Object Properties</a>



<a href="https://msdn.microsoft.com/0d0c6b3d-23bc-4628-a684-14bb9e18967f">Retrieving Properties for Multiple Objects</a>



<a href="https://msdn.microsoft.com/2332e3cc-087c-49cf-bde9-7f86f65158e7">Retrieving the Rendering Capabilities Supported by a Device</a>



<a href="https://msdn.microsoft.com/0686ba54-4782-42a4-8fdb-2325fc8d8bc2">Setting Properties for Multiple Objects</a>



<a href="https://msdn.microsoft.com/1c003534-96b4-419b-94d1-73b5ffa2eba1">Setting Properties for a Single Object</a>



<a href="https://msdn.microsoft.com/76069097-a513-42f7-bdcc-a65714e95f0a">Transferring Content from the Device to a PC</a>



<a href="https://msdn.microsoft.com/f762a571-83ea-4999-ad49-a51044bc790d">Writing Content-Object Properties</a>
 

 

