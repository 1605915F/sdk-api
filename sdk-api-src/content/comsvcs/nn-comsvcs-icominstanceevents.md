---
UID: NN:comsvcs.IComInstanceEvents
title: IComInstanceEvents
author: windows-sdk-content
description: Notifies the subscriber of an object's creation or release.
old-location: cos\icominstanceevents.htm
tech.root: cossdk
ms.assetid: 11e4559e-04c5-4fa9-b618-458ca7daf00e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IComInstanceEvents, IComInstanceEvents interface [COM+], IComInstanceEvents interface [COM+],described, _dtc_IComInstanceEvents, comsvcs/IComInstanceEvents, cos.icominstanceevents
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IComInstanceEvents
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IComInstanceEvents interface


## -description


Notifies the subscriber of an object's creation or release. The events are published to the subscriber using the <a href="https://msdn.microsoft.com/en-us/library/ms679237(v=VS.85).aspx">COM+ Events</a> service, a loosely coupled events system that stores event information from different publishers in an event store in the COM+ catalog.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IComInstanceEvents</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IComInstanceEvents</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IComInstanceEvents</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4f3457f6-4956-4411-b38b-46c7d84d342d">OnObjectCreate</a>
</td>
<td align="left" width="63%">
Generated when an object is created by a client.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms680535(v=VS.85).aspx">OnObjectDestroy</a>
</td>
<td align="left" width="63%">
Generated when an object is released by a client.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms679237(v=VS.85).aspx">COM+ Events</a>



<a href="https://msdn.microsoft.com/en-us/library/ms678896(v=VS.85).aspx">COM+ Instrumentation</a>
 

 

