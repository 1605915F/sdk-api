---
UID: NF:uianimation.IUIAnimationTransition.GetDuration
title: IUIAnimationTransition::GetDuration (uianimation.h)
author: windows-sdk-content
description: Gets the duration of the transition.
old-location: uianimation\iuianimationtransition_getduration.htm
tech.root: UIAnimation
ms.assetid: cc46ca31-3146-4d93-b859-79fe5e1fea08
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetDuration, GetDuration method [Windows Animation], GetDuration method [Windows Animation],IUIAnimationTransition interface, IUIAnimationTransition interface [Windows Animation],GetDuration method, IUIAnimationTransition.GetDuration, IUIAnimationTransition::GetDuration, uianimation.iuianimationtransition_getduration, uianimation/IUIAnimationTransition::GetDuration
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
 - IUIAnimationTransition.GetDuration
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationTransition::GetDuration


## -description


Gets the duration of the transition.


## -parameters




### -param duration [out]

The duration of the transition, in seconds.


## -returns



If the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>UI_E_VALUE_NOT_DETERMINED</b></dt>
</dl>
</td>
<td width="60%">
The requested value for the duration cannot be determined.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>UI_E_STORYBOARD_ACTIVE</b></dt>
</dl>
</td>
<td width="60%">
The storyboard for this transition is currently in the schedule.

</td>
</tr>
</table>
 




## -remarks



An application should typically call the <a href="https://msdn.microsoft.com/5cb22573-a318-4682-bc82-0a81c9dbdcbe">IUIAnimationTransition::IsDurationKnown</a> method before calling this method. This method should not be called when the storyboard to which the transition has been added is scheduled or playing.


#### Examples

The following shows how to get the duration of a transition.


```cpp
hr = pTransition->IsDurationKnown();
if (SUCCEEDED(hr))
{
    bool fDurationKnown = (hr == S_OK); 
    if (fDurationKnown)
    {
        UI_ANIMATION_SECONDS duration;
        hr = pTransition->GetDuration(&duration);
        if (SUCCEEDED(hr))
        {        
            ...
        }
    }
    else
    {
        ...
    }
}
```





## -see-also




<a href="https://msdn.microsoft.com/99804a2f-82c9-494c-b75d-69e66f1e49ef">IUIAnimationTransition</a>



<a href="https://msdn.microsoft.com/5cb22573-a318-4682-bc82-0a81c9dbdcbe">IUIAnimationTransition::IsDurationKnown</a>
 

 

