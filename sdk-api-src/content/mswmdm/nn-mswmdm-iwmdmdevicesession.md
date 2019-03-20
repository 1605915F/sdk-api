---
UID: NN:mswmdm.IWMDMDeviceSession
title: IWMDMDeviceSession (mswmdm.h)
author: windows-sdk-content
description: The IWMDMDeviceSession interface improves the efficiency of device operations by bundling multiple operations into one session.
old-location: wmdm\iwmdmdevicesession.htm
tech.root: WMDM
ms.assetid: 37a57fbe-d0f8-44ee-b6c5-2c6a34e12f2b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMDMDeviceSession, IWMDMDeviceSession interface [windows Media Device Manager], IWMDMDeviceSession interface [windows Media Device Manager],described, IWMDMDeviceSessionInterface, mswmdm/IWMDMDeviceSession, wmdm.iwmdmdevicesession
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
 - IWMDMDeviceSession
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMDMDeviceSession interface


## -description



The <b>IWMDMDeviceSession</b> interface improves the efficiency of device operations by bundling multiple operations into one session. Using a single session allows Windows Media Device Manager to handle various operations, such as acquiring a device certificate, once over several operations.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMDMDeviceSession</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMDMDeviceSession</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMDMDeviceSession</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7077e594-58ed-497d-893d-81eeb317b274">BeginSession</a>
</td>
<td align="left" width="63%">
Begins a device session.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/f587a20a-936f-49a4-8e56-2e05b3d295f6">EndSession</a>
</td>
<td align="left" width="63%">
Ends a device session.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/bea867d6-a875-4150-9958-7f683cd215b9">Interfaces for Applications</a>
 

 

