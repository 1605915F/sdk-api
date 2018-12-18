---
UID: NF:tapi3if.ITCallInfo2.get_EventFilter
title: ITCallInfo2::get_EventFilter
author: windows-sdk-content
description: The get_EventFilter method gets the event filter information applicable to this call.
old-location: tapi3\itcallinfo2_get_eventfilter.htm
tech.root: tapi
ms.assetid: 21f4f7ae-2bba-424b-889f-4b43e9416b33
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITCallInfo2 interface [TAPI 2.2],get_EventFilter method, ITCallInfo2.get_EventFilter, ITCallInfo2::get_EventFilter, _tapi3_itcallinfo2_get_eventfilter, get_EventFilter, get_EventFilter method [TAPI 2.2], get_EventFilter method [TAPI 2.2],ITCallInfo2 interface, tapi3.itcallinfo2_get_eventfilter, tapi3if/ITCallInfo2::get_EventFilter
ms.topic: method
req.header: tapi3if.h
req.include-header: Tapi3.h
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
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITCallInfo2.get_EventFilter
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITCallInfo2::get_EventFilter


## -description


The 
<b>get_EventFilter</b> method gets the event filter information applicable to this call.


## -parameters




### -param TapiEvent [in]

The 
<a href="https://msdn.microsoft.com/94faa4a1-7d86-48bc-9e94-f2b8f83f5280">TAPI_EVENT</a> descriptor of event type information being checked.


### -param lSubEvent [in]

Subevent descriptor.


### -param pEnable [out]

VARIANT_TRUE if notifications are being sent on this event type for this call.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/20f7b20e-37f8-49f7-ae9d-83a9b9f574b6">ITCallInfo2</a>
 

 

