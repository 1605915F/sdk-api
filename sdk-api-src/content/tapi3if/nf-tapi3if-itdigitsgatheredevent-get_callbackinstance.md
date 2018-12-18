---
UID: NF:tapi3if.ITDigitsGatheredEvent.get_CallbackInstance
title: ITDigitsGatheredEvent::get_CallbackInstance
author: windows-sdk-content
description: The get_CallbackInstance method gets a pointer to the application's callback function that will process the event.
old-location: tapi3\itdigitsgatheredevent_get_callbackinstance.htm
tech.root: tapi
ms.assetid: 28c613bc-8320-43b5-a9b3-b6a47876d7dd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ITDigitsGatheredEvent interface [TAPI 2.2],get_CallbackInstance method, ITDigitsGatheredEvent.get_CallbackInstance, ITDigitsGatheredEvent::get_CallbackInstance, _tapi3_itdigitsgatheredevent_get_callbackinstance, get_CallbackInstance, get_CallbackInstance method [TAPI 2.2], get_CallbackInstance method [TAPI 2.2],ITDigitsGatheredEvent interface, tapi3.itdigitsgatheredevent_get_callbackinstance, tapi3if/ITDigitsGatheredEvent::get_CallbackInstance
ms.topic: method
req.header: tapi3if.h
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
 - ITDigitsGatheredEvent.get_CallbackInstance
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ITDigitsGatheredEvent::get_CallbackInstance


## -description


The 
<b>get_CallbackInstance</b> method gets a pointer to the application's callback function that will process the event.


## -parameters




### -param plCallbackInstance [out]

Pointer to the callback instance returned by 
<a href="https://msdn.microsoft.com/335deb2c-7700-4101-b6fa-f7fe0f248307">ITTAPI::RegisterCallNotifications</a>.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>plCallbackInstance</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/2d710bea-a0fd-492b-81a3-03b741685c91">ITDigitsGatheredEvent</a>
 

 

