---
UID: NF:portabledeviceapi.IPortableDeviceServiceCapabilities.GetMethodAttributes
title: IPortableDeviceServiceCapabilities::GetMethodAttributes (portabledeviceapi.h)
author: windows-sdk-content
description: Retrieves the attributes used to describe a given method.
old-location: wpdsdk\iportabledeviceservicecapabilities_getmethodattributes.htm
tech.root: wpd_sdk
ms.assetid: 4cd125ea-545f-461b-90e1-88d3e3a6c032
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetMethodAttributes, GetMethodAttributes method [Windows Portable Devices SDK], GetMethodAttributes method [Windows Portable Devices SDK],IPortableDeviceServiceCapabilities interface, IPortableDeviceServiceCapabilities interface [Windows Portable Devices SDK],GetMethodAttributes method, IPortableDeviceServiceCapabilities.GetMethodAttributes, IPortableDeviceServiceCapabilities::GetMethodAttributes, portabledeviceapi/IPortableDeviceServiceCapabilities::GetMethodAttributes, wpdsdk.iportabledeviceservicecapabilities_getmethodattributes
ms.topic: method
req.header: portabledeviceapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: PortableDeviceAPI.idl
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
 - PortableDeviceAPI.h
api_name:
 - IPortableDeviceServiceCapabilities.GetMethodAttributes
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPortableDeviceServiceCapabilities::GetMethodAttributes


## -description


The <b>GetMethodAttributes</b> method retrieves the attributes used to describe a given method.


## -parameters




### -param Method [in]

The method whose attributes are retrieved.


### -param ppAttributes [out]

The <a href="https://msdn.microsoft.com/a73cbb4e-15d2-4c8d-9267-aaec9a0fd09f">IPortableDeviceValues</a> interface that receives the list of attributes.


## -returns



If the method succeeds, it returns <b>S_OK</b>. Any other <b>HRESULT</b> value indicates that the call failed. 
          




## -remarks



Possible attributes include the <a href="https://msdn.microsoft.com/en-us/library/Dd389006(v=VS.85).aspx">WPD_METHOD_ATTRIBUTE_NAME</a>, <b>WPD_METHOD_ATTRIBUTE_ASSOCIATED_FORMAT</b>, <b>WPD_METHOD_ATTRIBUTE_ACCESS</b>, and <a href="https://msdn.microsoft.com/en-us/library/Dd389067(v=VS.85).aspx">WPD_METHOD_ATTRIBUTE_PARAMETERS</a> properties.
      


#### Examples

For an example of how to use this method, see <a href="https://msdn.microsoft.com/783a6552-9b22-4af4-9252-b443e2624687">Retrieving Supported Service Methods</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/47b8d3dd-ea12-461d-935d-2de2c0157f88">Device Interface GUIDs</a>



<a href="https://msdn.microsoft.com/d472d31c-90da-4ecc-9cf7-4474457a244f">IPortableDeviceServiceCapabilities Interface</a>



<a href="https://msdn.microsoft.com/a7708c60-758a-4fb6-8ef9-074ecdc9cf60">Method, Format, and Parameter Attributes</a>



<a href="https://msdn.microsoft.com/783a6552-9b22-4af4-9252-b443e2624687">Retrieving Supported Service Methods</a>
 

 

