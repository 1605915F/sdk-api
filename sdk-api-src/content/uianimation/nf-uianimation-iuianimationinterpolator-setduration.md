---
UID: NF:uianimation.IUIAnimationInterpolator.SetDuration
title: IUIAnimationInterpolator::SetDuration (uianimation.h)
author: windows-sdk-content
description: Sets the duration of the transition.
old-location: uianimation\iuianimationinterpolator_setduration.htm
tech.root: UIAnimation
ms.assetid: 79038ada-ebc2-4259-862a-d81403c2f6b8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUIAnimationInterpolator interface [Windows Animation],SetDuration method, IUIAnimationInterpolator.SetDuration, IUIAnimationInterpolator::SetDuration, SetDuration, SetDuration method [Windows Animation], SetDuration method [Windows Animation],IUIAnimationInterpolator interface, uianimation.iuianimationinterpolator_setduration, uianimation/IUIAnimationInterpolator::SetDuration
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
 - IUIAnimationInterpolator.SetDuration
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationInterpolator::SetDuration


## -description


Sets the duration of the transition.


## -parameters




### -param duration [in]

The duration of the transition.


## -returns



If the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.




## -remarks



Windows Animation calls this method only after calling the <a href="https://msdn.microsoft.com/a897caa9-8a03-465e-8b74-b4614efce00c">GetDependencies</a> method, and only if that call returns <b>UI_ANIMATION_DEPENDENCY_DURATION</b> as one of its <i>durationDependencies</i> flags.

Typically, an interpolator with a duration dependency will have a duration parameter in its associated creation method of <a href="https://msdn.microsoft.com/62aec8da-e067-4b61-9465-e07fb5b42b7f">IUIAnimationTransitionFactory</a>.  The interpolator should store its duration when first initialized and overwrite it when <b>SetDuration</b> is called.

Windows Animation always calls the <a href="https://msdn.microsoft.com/a1c5451a-b8d0-4eb7-883c-6bd1d585cb11">SetInitialValueAndVelocity</a> method to set the initial value and velocity before calling <b>SetDuration</b>, so a custom interpolator need not check whether the initial value and velocity have been set.

Windows Animation can call <a href="https://msdn.microsoft.com/a1c5451a-b8d0-4eb7-883c-6bd1d585cb11">SetInitialValueAndVelocity</a> and <b>SetDuration</b> multiple times with different parameters. Interpolators can cache internal state to improve performance, but they must update this cached state each time <b>SetInitialValueAndVelocity</b> is called and ensure that the results of subsequent calls to <b>SetDuration</b> reflect the updated state.




## -see-also




<a href="https://msdn.microsoft.com/8e1f2a9a-ab93-485a-83b2-baebb9ee4bcc">IUIAnimationInterpolator</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd317034(v=VS.85).aspx">UI_ANIMATION_DEPENDENCIES</a>



<a href="https://msdn.microsoft.com/0745b227-61c4-462e-8529-9402c9eaa70a">UI_ANIMATION_SECONDS</a>
 

 

