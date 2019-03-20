---
UID: NN:comsvcs.IComInstance2Events
title: IComInstance2Events (comsvcs.h)
author: windows-sdk-content
description: Notifies the subscriber if an object is created or released by a client.
old-location: cos\icominstance2events.htm
tech.root: cossdk
ms.assetid: 2fb2904d-7069-4303-bb3c-2caef9499c1e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComInstance2Events, IComInstance2Events interface [COM+], IComInstance2Events interface [COM+],described, _dtc_icominstance2events, comsvcs/IComInstance2Events, cos.icominstance2events
ms.topic: interface
req.header: comsvcs.h
req.include-header: 
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - ComSvcs.h
api_name:
 - IComInstance2Events
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComInstance2Events interface


## -description


Notifies the subscriber if an object is created or released by a client. The events are published to the subscriber using the <a href="https://msdn.microsoft.com/1e0570ae-9099-465a-9133-72aa7d574932">COM+ Events</a> service, a loosely coupled events system that stores event information from different publishers in an event store in the COM+ catalog.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IComInstance2Events</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IComInstance2Events</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IComInstance2Events</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b7c359b8-2d49-4982-836b-50d749758fa6">OnObjectCreate2</a>
</td>
<td align="left" width="63%">
Generated when a client creates an object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/eeaf62b1-4c25-4232-829b-b2b147575ce9">OnObjectDestroy2</a>
</td>
<td align="left" width="63%">
Generated when a client releases an object.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/1e0570ae-9099-465a-9133-72aa7d574932">COM+ Events</a>



<a href="https://msdn.microsoft.com/07f68734-a382-4fe5-86af-90805f61c68d">COM+ Instrumentation</a>
 

 

