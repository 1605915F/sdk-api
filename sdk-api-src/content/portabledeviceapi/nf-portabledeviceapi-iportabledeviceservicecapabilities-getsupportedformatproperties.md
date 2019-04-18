---
UID: NF:portabledeviceapi.IPortableDeviceServiceCapabilities.GetSupportedFormatProperties
title: IPortableDeviceServiceCapabilities::GetSupportedFormatProperties (portabledeviceapi.h)
author: windows-sdk-content
description: Retrieves the properties supported by the service for the specified format.
old-location: wpdsdk\iportabledeviceservicecapabilities_getsupportedformatproperties.htm
tech.root: wpd_sdk
ms.assetid: 80ce7975-c567-4c99-9eb5-6d494a0f1883
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSupportedFormatProperties, GetSupportedFormatProperties method [Windows Portable Devices SDK], GetSupportedFormatProperties method [Windows Portable Devices SDK],IPortableDeviceServiceCapabilities interface, IPortableDeviceServiceCapabilities interface [Windows Portable Devices SDK],GetSupportedFormatProperties method, IPortableDeviceServiceCapabilities.GetSupportedFormatProperties, IPortableDeviceServiceCapabilities::GetSupportedFormatProperties, portabledeviceapi/IPortableDeviceServiceCapabilities::GetSupportedFormatProperties, wpdsdk.iportabledeviceservicecapabilities_getsupportedformatproperties
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
req.idl: Portabledeviceapi.idl
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
 - portabledeviceapi.h
api_name:
 - IPortableDeviceServiceCapabilities.GetSupportedFormatProperties
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPortableDeviceServiceCapabilities::GetSupportedFormatProperties


## -description


The <b>GetSupportedFormatProperties</b> method retrieves the properties supported by the service for the specified format.


## -parameters




### -param Format [in]

The format whose properties are retrieved.


### -param ppKeys [out]

The <a href="https://msdn.microsoft.com/2460f5bc-6b1c-4e3b-bdb9-faaa6d6c87fd">IPortableDeviceKeyCollection</a> interface that receives the list of properties.


## -returns



If the method succeeds, it returns <b>S_OK</b>. Any other <b>HRESULT</b> value indicates that the call failed. 
          




## -remarks



The retrieved property collection is a superset of all properties supported by an object of the specified format.

An application can also retrieve the properties for an object by calling the <a href="https://msdn.microsoft.com/c6c42347-145c-4be7-bea6-34b13c211cb1">IPortableDeviceService::SendCommand</a> method with the <a href="https://msdn.microsoft.com/842bd4d6-0824-4597-bb5d-9ef8769055fb">WPD_COMMAND_OBJECT_PROPERTIES_GET_SUPPORTED</a> property passed as the command identifier. However, the <b>GetSupportedFormatProperties</b> method is typically faster than the <b>IPortableDeviceService::SendCommand</b> method.




## -see-also




<a href="https://msdn.microsoft.com/d472d31c-90da-4ecc-9cf7-4474457a244f">IPortableDeviceServiceCapabilities Interface</a>
 

 

