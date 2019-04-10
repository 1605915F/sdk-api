---
UID: NF:uianimation.IUIAnimationManager.Pause
title: IUIAnimationManager::Pause (uianimation.h)
author: windows-sdk-content
description: Pauses all animations.
old-location: uianimation\iuianimationmanager_pause.htm
tech.root: UIAnimation
ms.assetid: 52b11e79-9930-4fd8-84b4-152917090519
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IUIAnimationManager interface [Windows Animation],Pause method, IUIAnimationManager.Pause, IUIAnimationManager::Pause, Pause, Pause method [Windows Animation], Pause method [Windows Animation],IUIAnimationManager interface, uianimation.iuianimationmanager_pause, uianimation/IUIAnimationManager::Pause
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
 - IUIAnimationManager.Pause
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationManager::Pause


## -description


Pauses all animations.


## -parameters






## -returns



If the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.




## -remarks



When an animation manager is paused, its status is set to <b>UI_ANIMATION_MANAGER_IDLE</b>.




## -see-also




<a href="https://msdn.microsoft.com/21f16c65-90aa-4b1f-93bc-8ee0488c6ded">IUIAnimationManager</a>



<a href="https://msdn.microsoft.com/838140c3-12ca-4909-a0f8-713b5472e5a9">IUIAnimationManager::GetStatus</a>



<a href="https://msdn.microsoft.com/f29a9337-0ed0-46f8-ab77-8f82ab39d8df">IUIAnimationManager::Resume</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd317043(v=VS.85).aspx">UI_ANIMATION_MANAGER_STATUS</a>
 

 

