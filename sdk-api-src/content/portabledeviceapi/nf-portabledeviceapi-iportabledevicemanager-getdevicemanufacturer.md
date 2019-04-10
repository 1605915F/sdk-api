---
UID: NF:portabledeviceapi.IPortableDeviceManager.GetDeviceManufacturer
title: IPortableDeviceManager::GetDeviceManufacturer (portabledeviceapi.h)
author: windows-sdk-content
description: Retrieves the name of the device manufacturer.
old-location: wpdsdk\iportabledevicemanager_getdevicemanufacturer.htm
tech.root: wpd_sdk
ms.assetid: 2bd64da1-819d-430c-ab66-ab3b8e6c48f6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetDeviceManufacturer, GetDeviceManufacturer method [Windows Portable Devices SDK], GetDeviceManufacturer method [Windows Portable Devices SDK],IPortableDeviceManager interface, IPortableDeviceManager interface [Windows Portable Devices SDK],GetDeviceManufacturer method, IPortableDeviceManager.GetDeviceManufacturer, IPortableDeviceManager::GetDeviceManufacturer, IPortableDeviceManagerGetDeviceManufacturer, portabledeviceapi/IPortableDeviceManager::GetDeviceManufacturer, wpdsdk.iportabledevicemanager_getdevicemanufacturer
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
 - IPortableDeviceManager.GetDeviceManufacturer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPortableDeviceManager::GetDeviceManufacturer


## -description



Retrieves the name of the device manufacturer.




## -parameters




### -param pszPnPDeviceID [in]

Pointer to a null-terminated string that contains the device's Plug and Play ID. You can retrieve a list of Plug and Play names of all devices that are connected to the computer by calling <a href="https://msdn.microsoft.com/5061b3c0-8b93-480d-b1c6-0a6b616a2c8d">GetDevices</a>.


### -param pDeviceManufacturer [in, out]

A caller-allocated buffer that holds the name of the device manufacturer. To learn the required size for this parameter, first call this method with this parameter set to <b>NULL</b> and <i>pcchDeviceManufacturer</i> set to <b>0</b>; the method will succeed and set <i>pcchDeviceManufacturer</i> to the required buffer size to hold the device-friendly name, including the termination character.


### -param pcchDeviceManufacturer [in, out]

On input, the maximum number of characters that <i>pDeviceManufacturer</i> can hold, not including the termination character. On output, the number of characters returned by <i>pDeviceManufacturer</i>, not including the termination character.


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
<dt><b>HRESULT_FROM_WIN32(ERROR_INSUFFICIENT_BUFFER)</b></dt>
</dl>
</td>
<td width="60%">
The supplied buffer is not large enough to hold the device description. (Refer to the value returned in <i>pcchDeviceDescription</i> for the required size.)

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>HRESULT_FROM_WIN32(ERROR_INVALID_DATA)</b></dt>
</dl>
</td>
<td width="60%">
The device description could not be found.

</td>
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
 




## -see-also




<a href="https://msdn.microsoft.com/11cd5b2b-e8f8-4ba1-8527-f7a403f399d5">IPortableDeviceManager Interface</a>



<a href="https://msdn.microsoft.com/5061b3c0-8b93-480d-b1c6-0a6b616a2c8d">IPortableDeviceManager::GetDevices</a>
 

 

