---
UID: NF:wmsdkidl.IWMRegisteredDevice.GetAttributeCount
title: IWMRegisteredDevice::GetAttributeCount
author: windows-sdk-content
description: The GetAttributeCount method retrieves the total number of attributes associated with the device.
old-location: wmformat\iwmregistereddevice_getattributecount.htm
tech.root: wmformat
ms.assetid: 6032cb18-4c4a-4cd7-905e-5cb390bfc37b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAttributeCount, GetAttributeCount method [windows Media Format], GetAttributeCount method [windows Media Format],IWMRegisteredDevice interface, IWMRegisteredDevice interface [windows Media Format],GetAttributeCount method, IWMRegisteredDevice.GetAttributeCount, IWMRegisteredDevice::GetAttributeCount, IWMRegisteredDeviceGetAttributeCount, wmformat.iwmregistereddevice_getattributecount, wmsdkidl/IWMRegisteredDevice::GetAttributeCount
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
 - IWMRegisteredDevice.GetAttributeCount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMRegisteredDevice::GetAttributeCount


## -description



The <b>GetAttributeCount</b> method retrieves the total number of attributes associated with the device.




## -parameters




### -param pcAttributes [out]

Address of a variable that receives the number of attributes.


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



To enumerate the device attributes, first call this method and then call <a href="https://msdn.microsoft.com/02a582d4-329e-47e3-9dbe-dba8a3e4b4b3">GetAttributeByIndex</a> for index values from zero through one less than the total number of attributes.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd743621(v=VS.85).aspx">IWMRegisteredDevice Interface</a>
 

 

