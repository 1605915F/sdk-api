---
UID: NN:strmif.IAMTVAudioNotification
title: IAMTVAudioNotification (strmif.h)
author: windows-sdk-content
description: Note  This callback interface has been deprecated, because the TV Audio filter does not implement the callback mechanism. .
old-location: dshow\iamtvaudionotification.htm
tech.root: DirectShow
ms.assetid: 4f84586f-7384-4dd7-99ce-325fb609daae
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAMTVAudioNotification, IAMTVAudioNotification interface [DirectShow], IAMTVAudioNotification interface [DirectShow],described, IAMTVAudioNotificationInterface, dshow.iamtvaudionotification, strmif/IAMTVAudioNotification
ms.topic: interface
req.header: strmif.h
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
 - strmif.h
api_name:
 - IAMTVAudioNotification
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMTVAudioNotification interface


## -description



<div class="alert"><b>Note</b>  This callback interface has been deprecated, because the TV Audio filter does not implement the callback mechanism.</div>
<div> </div>



## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAMTVAudioNotification</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IAMTVAudioNotification</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IAMTVAudioNotification</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5282cbbf-5501-42eb-95ba-bf7b32792d56">OnEvent</a>
</td>
<td align="left" width="63%">
Handles events from a TV tuner card controlled by the <a href="https://msdn.microsoft.com/de340594-4410-4896-b206-0f47d4035bc1">IAMTVAudio</a> interface.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/5b798477-9b36-4f59-b9cc-2938b5e4009f">Deprecated Interfaces</a>
 

 

