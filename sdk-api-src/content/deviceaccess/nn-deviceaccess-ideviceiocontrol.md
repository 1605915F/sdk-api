---
UID: NN:deviceaccess.IDeviceIoControl
title: IDeviceIoControl
author: windows-sdk-content
description: Sends a control code to a device driver.This action causes the device to perform the corresponding operation.
old-location: deviceaccess\ideviceiocontrol.htm
tech.root: deviceaccess
ms.assetid: d285e04e-04d0-4c2a-b9f0-72eebebf4f4b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDeviceIoControl, IDeviceIoControl interface [Device Access Broker API], IDeviceIoControl interface [Device Access Broker API],described, deviceaccess.ideviceiocontrol, deviceaccess/IDeviceIoControl
ms.topic: interface
req.header: deviceaccess.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Deviceaccess.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Deviceaccess.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Deviceaccess.lib
 - Deviceaccess.dll
api_name:
 - IDeviceIoControl
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDeviceIoControl interface


## -description


Sends a control code to a device driver.This action causes the device to perform the corresponding operation. 


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDeviceIoControl</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IDeviceIoControl</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDeviceIoControl</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/476a84c8-4065-4a4f-ad74-68cbbbabd5dd">CancelOperation</a>
</td>
<td align="left" width="63%">
Attempts to cancel a previously issued call by using the <a href="https://msdn.microsoft.com/550eadd0-c03b-40b3-9f08-639085365f4b">DeviceIoControlAsync</a> method.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/550eadd0-c03b-40b3-9f08-639085365f4b">DeviceIoControlAsync</a>
</td>
<td align="left" width="63%">
Sends an asynchronous device I/O control request to the device interface that's specified by the call to the <a href="https://msdn.microsoft.com/082d6297-20ac-4557-8205-0451482a5758">CreateDeviceAccessInstance</a> function.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7b17ab14-e9bb-40be-a463-ca9031ba9bb3">DeviceIoControlSync</a>
</td>
<td align="left" width="63%">
Sends a synchronous device I/O control request to the device interface that's specified by the call to <a href="https://msdn.microsoft.com/082d6297-20ac-4557-8205-0451482a5758">CreateDeviceAccessInstance</a>.

</td>
</tr>
</table> 

