---
UID: NF:uianimation.IUIAnimationStoryboard2.AddKeyframeAfterTransition
title: IUIAnimationStoryboard2::AddKeyframeAfterTransition (uianimation.h)
author: windows-sdk-content
description: Adds a keyframe at the end of the specified transition.
old-location: uianimation\iuianimationstoryboard2_addkeyframeaftertransition.htm
tech.root: UIAnimation
ms.assetid: F5D13D36-1AEE-4D47-9683-A428E9ADF1D6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddKeyframeAfterTransition, AddKeyframeAfterTransition method [Windows Animation], AddKeyframeAfterTransition method [Windows Animation],IUIAnimationStoryboard2 interface, IUIAnimationStoryboard2 interface [Windows Animation],AddKeyframeAfterTransition method, IUIAnimationStoryboard2.AddKeyframeAfterTransition, IUIAnimationStoryboard2::AddKeyframeAfterTransition, uianimation.iuianimationstoryboard2_addkeyframeaftertransition, uianimation/IUIAnimationStoryboard2::AddKeyframeAfterTransition
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
 - IUIAnimationStoryboard2.AddKeyframeAfterTransition
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationStoryboard2::AddKeyframeAfterTransition


## -description


Adds a keyframe at the end of the specified transition.


## -parameters




### -param transition [in]

The transition after which a keyframe is to be added.


### -param keyframe [out]

The keyframe to be added.


## -returns



If this method succeeds, it returns S_OK. Otherwise, it returns an  <b>HRESULT</b> error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>UI_E_TRANSITION_NOT_IN_STORYBOARD</b></dt>
</dl>
</td>
<td width="60%">
The transition has not been added to the storyboard.

</td>
</tr>
</table>
 

See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.




## -remarks



A keyframe represents a moment in time within a storyboard and can be used to specify the start and end times of transitions. Because keyframes can be added at the ends of transitions, their offsets from the start of the storyboard may not be known until the storyboard is playing.




## -see-also




<a href="https://msdn.microsoft.com/507B6C2B-92C6-4AEB-82D5-3F14A332D41F">IUIAnimationStoryboard2</a>



<a href="https://msdn.microsoft.com/6AB47BC1-4437-4191-8B66-8545EB4102A9">IUIAnimationStoryboard2::AddKeyframeAtOffset</a>



<a href="https://msdn.microsoft.com/BFC05D67-EE1C-489E-9A8C-10F0AAB24A0A">IUIAnimationStoryboard2::AddTransition</a>



<a href="https://msdn.microsoft.com/F4DAB833-E857-4FD8-87E2-8F32AF460F90">IUIAnimationStoryboard2::AddTransitionAtKeyframe</a>



<a href="https://msdn.microsoft.com/55AEA5EA-7D9E-4669-8315-7A6F4428EDF9">IUIAnimationStoryboard2::AddTransitionBetweenKeyframes</a>



<a href="https://msdn.microsoft.com/CACB8053-7716-42E4-9C3B-9CCBBC30808A">IUIAnimationTransition2</a>



<a href="https://msdn.microsoft.com/92C10ED5-DCE6-4B1D-8608-E2C3C6AD97BA">IUIAnimationTransitionLibrary2</a>



<a href="https://msdn.microsoft.com/4ac3d524-35a6-4cb9-a468-b7f88500a49c">UI_ANIMATION_KEYFRAME</a>
 

 

