---
UID: NN:eventsys.IMultiInterfaceEventControl
title: IMultiInterfaceEventControl (eventsys.h)
author: windows-sdk-content
description: Controls the behavior of an event object, the object that fires an event to its subscribers.
old-location: cos\imultiinterfaceeventcontrol.htm
tech.root: cossdk
ms.assetid: e603f68a-881c-468d-a3d3-738f43400e01
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMultiInterfaceEventControl, IMultiInterfaceEventControl interface [COM+], IMultiInterfaceEventControl interface [COM+],described, _cos_IMultiInterfaceEventControl, cos.imultiinterfaceeventcontrol, eventsys/IMultiInterfaceEventControl
ms.topic: interface
req.header: eventsys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: EventSys.idl
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
 - EventSys.h
api_name:
 - IMultiInterfaceEventControl
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMultiInterfaceEventControl interface


## -description


Controls the behavior of an event object, the object that fires an event to its subscribers. The <b>IMultiInterfaceEventControl</b> interface differs from the <a href="https://msdn.microsoft.com/8b2fba30-3ede-466f-ad3b-2de2175a088b">IEventControl</a> interface in that it supports multiple event interfaces for the event object.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMultiInterfaceEventControl</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IMultiInterfaceEventControl</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>IMultiInterfaceEventControl</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/38b1d0fe-c32e-41d5-a0c1-2b4e72908fce">GetSubscriptions</a>
</td>
<td align="left" width="63%">
Retrieves the collection of subscription objects associated with an event method.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/31d544d4-8cac-46ae-9db7-c5b366ac6b2f">SetDefaultQuery</a>
</td>
<td align="left" width="63%">
Establishes a default query to be used when a publisher filter is not associated with an event method.


</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/0eb52937-3bd8-45ab-b4ba-c0264c47c909">SetMultiInterfacePublisherFilter</a>
</td>
<td align="left" width="63%">
Assigns a publisher filter to an event method at run time.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMultiInterfaceEventControl</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="10%">Access type</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/152f78d9-4292-45e8-a908-5d2b0368f507">AllowInprocActivation</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
Indicates whether subscribers can be activated in the publisher's process.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/c26cce66-e713-42f7-9716-385b59085977">FireInParallel</a>


</td>
<td align="left" width="10%">
Read/write

</td>
<td align="left" width="63%">
Indicates whether events can be delivered to two or more subscribers in parallel.

</td>
</tr>
</table> 

