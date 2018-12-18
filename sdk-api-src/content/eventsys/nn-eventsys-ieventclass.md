---
UID: NN:eventsys.IEventClass
title: IEventClass
author: windows-sdk-content
description: Associates a class of event objects with the event interface those objects implement.
old-location: cos\ieventclass.htm
tech.root: cossdk
ms.assetid: e8c1fcd1-59fb-49d6-94b9-52b7c8551651
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEventClass, IEventClass interface [COM+], IEventClass interface [COM+],described, _cos_IEventClass, cos.ieventclass, eventsys/IEventClass
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
req.idl: Eventsys.idl
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
 - eventsys.h
api_name:
 - IEventClass
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEventClass interface


## -description


Associates a class of event objects with the event interface those objects implement.

<b>IEventClass</b> is the interface that is implemented by the CLSID_CEventClass objects, which are different than event class objects that are co-created by a publisher for the purpose of firing events.

An event object implements the <a href="https://msdn.microsoft.com/e603f68a-881c-468d-a3d3-738f43400e01">IMultiInterfaceEventControl</a> event interface. While this object can be used to configure event classes in the event store, the preferred method is to use the COM+ Administration interfaces. However, not all of the properties exposed by the <b>IEventClass</b> interface are available through the COM+ Administration interfaces.


## -see-also




<a href="https://msdn.microsoft.com/0e04cd6f-1f8b-4bdf-92b0-5baddeb361b5">COM+ Administration Interfaces</a>
 

 

