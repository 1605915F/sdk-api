---
UID: NN:mswmdm.IMDSPEnumDevice
title: IMDSPEnumDevice
author: windows-sdk-content
description: The IMDSPEnumDevice interface is used to enumerate the media devices.
old-location: wmdm\imdspenumdevice.htm
tech.root: WMDM
ms.assetid: 9a296937-6f8b-4f04-989f-3a5d4c6f7b85
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMDSPEnumDevice, IMDSPEnumDevice interface [windows Media Device Manager], IMDSPEnumDevice interface [windows Media Device Manager],described, IMDSPEnumDeviceInterface, mswmdm/IMDSPEnumDevice, wmdm.imdspenumdevice
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: mswmdm.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mswmdm.h
api_name:
 - IMDSPEnumDevice
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMDSPEnumDevice interface


## -description



The <b>IMDSPEnumDevice</b> interface is used to enumerate the media devices. For more information on enumeration, see the Microsoft COM documentation on the COM page at the <a href="http://go.microsoft.com/fwlink/p/?linkid=3282">Microsoft Web site</a>. The <b>IMDSPEnumDevice</b> interface is implemented on the device enumerator object. The only valid way to create a device enumerator object is to call <a href="https://msdn.microsoft.com/a3d4e404-7441-4a61-b2bb-ca373eb79b99">IMDServiceProvider::EnumDevices</a>. If the device implements <a href="https://msdn.microsoft.com/f724ef14-c572-41ca-a56b-fde85d7620e0">IMDServiceProvider2::CreateDevice</a>, this enumerator should enumerate only non-Plug and Play devices. The device enumerator should enumerate only the devices that are attached to the computer and are supported by the service provider.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMDSPEnumDevice</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IMDSPEnumDevice</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMDSPEnumDevice</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/fe6b8766-4f63-4a6c-b7dd-39a304679185">Clone</a>
</td>
<td align="left" width="63%">
Creates another enumerator that contains the same enumeration state as the current one.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/137bcc3b-8c6e-4512-b564-a32af437f69a">Next</a>
</td>
<td align="left" width="63%">
Returns a pointer to the next <a href="https://msdn.microsoft.com/98f16547-4d8a-4422-ba08-c3c678142492">IMDSPDevice</a> interface.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7edd0d45-aeae-4bc8-b4d4-f74bcb403ef9">Reset</a>
</td>
<td align="left" width="63%">
Resets the enumeration sequence to the beginning.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/17b4e680-7f55-4f96-a0ca-acfda9f17784">Skip</a>
</td>
<td align="left" width="63%">
Skips over the next specified number of media device interface(s) in the enumeration sequence.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/98f16547-4d8a-4422-ba08-c3c678142492">IMDSPDevice Interface</a>



<a href="https://msdn.microsoft.com/a3d4e404-7441-4a61-b2bb-ca373eb79b99">IMDServiceProvider::EnumDevices</a>



<a href="https://msdn.microsoft.com/bd61c5fa-047c-4d93-bae1-f3433696b95b">Interfaces for Service Providers</a>
 

 

