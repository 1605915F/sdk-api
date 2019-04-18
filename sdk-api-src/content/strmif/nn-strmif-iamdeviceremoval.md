---
UID: NN:strmif.IAMDeviceRemoval
title: IAMDeviceRemoval (strmif.h)
author: windows-sdk-content
description: The IAMDeviceRemoval interface provides a way for the Filter Graph Manager to register for device removal events for a capture device.
old-location: dshow\iamdeviceremoval.htm
tech.root: DirectShow
ms.assetid: 3d67f577-9d85-47ca-b887-f259e9acc964
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IAMDeviceRemoval, IAMDeviceRemoval interface [DirectShow], IAMDeviceRemoval interface [DirectShow],described, IAMDeviceRemovalInterface, dshow.iamdeviceremoval, strmif/IAMDeviceRemoval
ms.topic: interface
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IAMDeviceRemoval
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAMDeviceRemoval interface


## -description



The <code>IAMDeviceRemoval</code> interface provides a way for the Filter Graph Manager to register for device removal events for a capture device. The KsProxy filter exposes this interface. (See <a href="https://msdn.microsoft.com/97432b99-e89b-4d69-963d-a959f887e580">WDM Video Capture Filter</a>.)

Applications typically do not use this interface, and third-party filters do not need to implement this interface. To get a pointer to this interface, call <b>QueryInterface</b> on the KsProxy filter.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAMDeviceRemoval</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IAMDeviceRemoval</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IAMDeviceRemoval</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ec3628cf-fcb4-46c4-9de1-79bf1259c3db">DeviceInfo</a>
</td>
<td align="left" width="63%">
Retrieves information about the device

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/cf868f5d-3ec1-4c01-9154-27420d136fe5">Disassociate</a>
</td>
<td align="left" width="63%">
Disassociates the KsProxy filter from the device by closing the device handle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/214b98c7-4143-4466-a359-1e9c9e4c778d">Reassociate</a>
</td>
<td align="left" width="63%">
Reassociates the KsProxy filter with the device.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/5efd174f-2eb1-44e6-97e3-b73c7c52fef1">Interfaces</a>
 

 

