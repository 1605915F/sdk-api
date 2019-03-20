---
UID: NF:wmsdkidl.IWMRegisteredDevice.GetDeviceCertificate
title: IWMRegisteredDevice::GetDeviceCertificate (wmsdkidl.h)
author: windows-sdk-content
description: The GetDeviceCertificate method retrieves the certificate of the device.
old-location: wmformat\iwmregistereddevice_getdevicecertificate.htm
tech.root: wmformat
ms.assetid: 80313abc-2212-4b1a-9d4e-9f3015370ea7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDeviceCertificate, GetDeviceCertificate method [windows Media Format], GetDeviceCertificate method [windows Media Format],IWMRegisteredDevice interface, IWMRegisteredDevice interface [windows Media Format],GetDeviceCertificate method, IWMRegisteredDevice.GetDeviceCertificate, IWMRegisteredDevice::GetDeviceCertificate, IWMRegisteredDeviceGetDeviceCertificate, wmformat.iwmregistereddevice_getdevicecertificate, wmsdkidl/IWMRegisteredDevice::GetDeviceCertificate
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only],Windows Media Format 9.5 SDK
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WMStubDRM.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - WMStubDRM.lib
 - WMStubDRM.dll
api_name:
 - IWMRegisteredDevice.GetDeviceCertificate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMRegisteredDevice::GetDeviceCertificate


## -description



The <b>GetDeviceCertificate</b> method retrieves the certificate of the device.




## -parameters




### -param ppCertificate [out]

Address of a variable that receives a pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dd743243(v=VS.85).aspx">INSSBuffer</a> interface of the buffer object that contains the certificate data.


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



The device certificate contains protection information related to the device.

Together, the device certificate and the device serial number uniquely identify the device. Manufacturers are encouraged to use a separate certificate for each device. However, a manufacturer may share a certificate between all devices of a particular type, differentiating individual devices by serial number.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd743621(v=VS.85).aspx">IWMRegisteredDevice Interface</a>
 

 

