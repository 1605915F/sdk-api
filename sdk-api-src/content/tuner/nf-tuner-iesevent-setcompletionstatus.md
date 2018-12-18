---
UID: NF:tuner.IESEvent.SetCompletionStatus
title: IESEvent::SetCompletionStatus
author: windows-sdk-content
description: Sets the completion status for an event that is derived from the IESEvent interface.
old-location: mstv\iesevent_setcompletionstatus.htm
tech.root: mstv
ms.assetid: 2e8d5a94-6fa1-453b-bbd4-396d60bb2aa0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IESEvent interface [Microsoft TV Technologies],SetCompletionStatus method, IESEvent.SetCompletionStatus, IESEvent::SetCompletionStatus, SetCompletionStatus, SetCompletionStatus method [Microsoft TV Technologies], SetCompletionStatus method [Microsoft TV Technologies],IESEvent interface, mstv.iesevent_setcompletionstatus, tuner/IESEvent::SetCompletionStatus
ms.topic: method
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
 - tuner.h
api_name:
 - IESEvent.SetCompletionStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IESEvent::SetCompletionStatus


## -description


Sets the completion status for an event that is derived from the <a href="https://msdn.microsoft.com/3c375480-c6df-4bb0-b417-5765b0bed9bf">IESEvent</a> interface. The device handling the event sets the completion status in the <b>IESEvent</b> object that is passed in a call to <a href="https://msdn.microsoft.com/3781e50c-ab19-4bfa-86d6-af12223019ca">IESEventService::FireESEvent</a>.
    

If an event originates from a PBDA device, the event object automatically calls the <a href="https://msdn.microsoft.com/en-us/library/Dd693346(v=VS.85).aspx">IBDA_EventingService::CompleteEvent</a> method with the result set in the <b>SetCompletionStatus</b> call at the time it is released.  If the client is a managed application, it should dispose of the event object immediately after it is finished with the event. This disposition ensures that the <b>IBDA_EventingService::CompleteEvent</b> method is called in a timely manner


## -parameters




### -param dwResult [in]

Completion status for the event.
          


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/3781e50c-ab19-4bfa-86d6-af12223019ca">FireESEvent</a>



<a href="https://msdn.microsoft.com/3c375480-c6df-4bb0-b417-5765b0bed9bf">IESEvent</a>
 

 

