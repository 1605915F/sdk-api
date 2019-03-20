---
UID: NF:evntprov.EventDescSetVersion
title: EventDescSetVersion function (evntprov.h)
author: windows-sdk-content
description: Sets the Version member of the event descriptor.
old-location: etw\eventdescsetversion_func.htm
tech.root: ETW
ms.assetid: f1d9fcb2-5a27-483b-b133-e8309b51165c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EventDescSetVersion, EventDescSetVersion function [ETW], base.eventdescsetversion_func, etw.eventdescsetversion_func, evntprov/EventDescSetVersion
ms.topic: function
req.header: evntprov.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - HeaderDef
api_location:
 - Evntprov.h
api_name:
 - EventDescSetVersion
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# EventDescSetVersion function


## -description


Sets the <b>Version</b> member of the event descriptor.


## -parameters




### -param EventDescriptor [in]

Event descriptor to modify. See <a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">EVENT_DESCRIPTOR</a>.


### -param Version [in]

Version that identifies the revision level of the event definition. The first version of an event is zero.


## -returns



The modified event descriptor.




## -remarks



This is a convenience macro for setting the member of the <a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">EVENT_DESCRIPTOR</a> structure.




## -see-also




<a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">EVENT_DESCRIPTOR</a>
 

 

