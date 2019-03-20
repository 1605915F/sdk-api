---
UID: NF:uianimation.IUIAnimationManager2.AbandonAllStoryboards
title: IUIAnimationManager2::AbandonAllStoryboards (uianimation.h)
author: windows-sdk-content
description: Abandons all active storyboards.
old-location: uianimation\iuianimationmanager2_abandonallstoryboards.htm
tech.root: UIAnimation
ms.assetid: E8DC71C0-CA68-4FD8-81CE-68450BF4EBA7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AbandonAllStoryboards, AbandonAllStoryboards method [Windows Animation], AbandonAllStoryboards method [Windows Animation],IUIAnimationManager2 interface, IUIAnimationManager2 interface [Windows Animation],AbandonAllStoryboards method, IUIAnimationManager2.AbandonAllStoryboards, IUIAnimationManager2::AbandonAllStoryboards, uianimation.iuianimationmanager2_abandonallstoryboards, uianimation/IUIAnimationManager2::AbandonAllStoryboards
ms.topic: method
req.header: uianimation.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8, Windows 7 and Platform Update for Windows 7 [desktop apps \| UWP apps]
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
 - IUIAnimationManager2.AbandonAllStoryboards
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationManager2::AbandonAllStoryboards


## -description


Abandons all active storyboards.


## -parameters






## -returns



If this method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.




## -remarks



Calling this method is equivalent to calling the <a href="https://msdn.microsoft.com/2350dbd0-3a67-4832-94dd-56adce80a387">IUIAnimationStoryboard::Abandon</a>method for each active storyboard.
         
         

A storyboard is considered active if a call to the <a href="https://msdn.microsoft.com/8ee9a17f-c57c-49df-950d-491e05ba8768">IUIAnimationStoryboard::GetStatus</a> method returns <a href="https://msdn.microsoft.com/en-us/library/Dd371971(v=VS.85).aspx">UI_ANIMATION_STORYBOARD_PLAYING</a> 
         or <a href="https://msdn.microsoft.com/en-us/library/Dd371971(v=VS.85).aspx">UI_ANIMATION_STORYBOARD_SCHEDULED</a>.




## -see-also




<a href="https://msdn.microsoft.com/BD7DAD23-2A7D-4EE7-9BCF-8380F928674D">IUIAnimationManager2</a>



<a href="https://msdn.microsoft.com/2350dbd0-3a67-4832-94dd-56adce80a387">IUIAnimationStoryboard::Abandon</a>



<a href="https://msdn.microsoft.com/8ee9a17f-c57c-49df-950d-491e05ba8768">IUIAnimationStoryboard::GetStatus</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd371971(v=VS.85).aspx">UI_ANIMATION_STORYBOARD_STATUS</a>
 

 

