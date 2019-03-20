---
UID: NF:uianimation.IUIAnimationTimerUpdateHandler.SetTimerClientEventHandler
title: IUIAnimationTimerUpdateHandler::SetTimerClientEventHandler (uianimation.h)
author: windows-sdk-content
description: Specifies a handler for timer client status change events.
old-location: uianimation\iuianimationtimerupdatehandler_settimerclienteventhandler.htm
tech.root: UIAnimation
ms.assetid: ce213fc5-1329-413f-abf1-a4ab7c78818e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUIAnimationTimerUpdateHandler interface [Windows Animation],SetTimerClientEventHandler method, IUIAnimationTimerUpdateHandler.SetTimerClientEventHandler, IUIAnimationTimerUpdateHandler::SetTimerClientEventHandler, SetTimerClientEventHandler, SetTimerClientEventHandler method [Windows Animation], SetTimerClientEventHandler method [Windows Animation],IUIAnimationTimerUpdateHandler interface, uianimation.iuianimationtimerupdatehandler_settimerclienteventhandler, uianimation/IUIAnimationTimerUpdateHandler::SetTimerClientEventHandler
ms.topic: method
req.header: uianimation.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAnimation.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: UIAnimation.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - UIAnimation.dll
api_name:
 - IUIAnimationTimerUpdateHandler.SetTimerClientEventHandler
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationTimerUpdateHandler::SetTimerClientEventHandler


## -description


Specifies a handler for timer client status change events.


## -parameters




### -param handler [in]

A handler for timer client events.  The specified object must implement
               <a href="https://msdn.microsoft.com/8ca8f7d8-e698-4c55-8241-5c8f7b47f0e8">IUIAnimationTimerUpdateHandler</a>.
            


## -returns



If the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.




## -remarks



If the update handler is already connected to the timer, this method returns <b>UI_E_TIMER_CLIENT_ALREADY_CONNECTED.</b>




## -see-also




<a href="https://msdn.microsoft.com/f155ed12-d493-48a0-9bdf-0e1e79cbcd38">IUIAnimationTimerUpdateHandler</a>



<a href="https://msdn.microsoft.com/c7383df5-dbd4-4cae-a682-47f84c2e8106">IUIAnimationTimerUpdateHandler::ClearTimerClientEventHandler</a>
 

 

