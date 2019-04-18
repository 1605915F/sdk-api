---
UID: NF:evntprov.EventDescSetKeyword
title: EventDescSetKeyword function (evntprov.h)
author: windows-sdk-content
description: Sets the Keyword member of the event descriptor.
old-location: etw\eventdescsetkeyword_func.htm
tech.root: ETW
ms.assetid: b1870a89-2e15-42b6-8441-82e6f9165540
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EventDescSetKeyword, EventDescSetKeyword function [ETW], base.eventdescsetkeyword_func, etw.eventdescsetkeyword_func, evntprov/EventDescSetKeyword
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
 - EventDescSetKeyword
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# EventDescSetKeyword function


## -description


Sets the <b>Keyword</b> member of the event descriptor.


## -parameters




### -param EventDescriptor [in]

Event descriptor to modify. See <a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">EVENT_DESCRIPTOR</a>.


### -param Keyword [in]

Keyword that is a bitmask that further defines the category of events to which the event belongs.


## -returns



The modified event descriptor.




## -remarks



This is a convenience macro for setting the member of the <a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">EVENT_DESCRIPTOR</a> structure.




## -see-also




<a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">EVENT_DESCRIPTOR</a>
 

 

