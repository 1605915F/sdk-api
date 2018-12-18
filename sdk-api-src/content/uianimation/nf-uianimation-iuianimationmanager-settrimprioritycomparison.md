---
UID: NF:uianimation.IUIAnimationManager.SetTrimPriorityComparison
title: IUIAnimationManager::SetTrimPriorityComparison
author: windows-sdk-content
description: Sets the priority comparison handler to be called to determine whether a scheduled storyboard can be trimmed.
old-location: uianimation\iuianimationmanager_settrimprioritycomparison.htm
tech.root: UIAnimation
ms.assetid: f4c81cc4-4c00-4f78-819d-55f79972fe46
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUIAnimationManager interface [Windows Animation],SetTrimPriorityComparison method, IUIAnimationManager.SetTrimPriorityComparison, IUIAnimationManager::SetTrimPriorityComparison, SetTrimPriorityComparison, SetTrimPriorityComparison method [Windows Animation], SetTrimPriorityComparison method [Windows Animation],IUIAnimationManager interface, uianimation.iuianimationmanager_settrimprioritycomparison, uianimation/IUIAnimationManager::SetTrimPriorityComparison
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
 - IUIAnimationManager.SetTrimPriorityComparison
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationManager::SetTrimPriorityComparison


## -description


Sets the priority comparison handler to be called to determine whether a scheduled storyboard can be trimmed.


## -parameters




### -param comparison [in, optional]

The priority comparison handler for trimming.  
               
               The specified object must implement the
               <a href="https://msdn.microsoft.com/65311cf0-f8d4-4d2c-bd4d-585ae5d921df">IUIAnimationPriorityComparison</a> interface or be <b>NULL</b>.
            See Remarks.


## -returns



If the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.
            




## -remarks



Setting a priority comparison handler with this method enables the application to indicate when  scheduling conflicts can be resolved by trimming the scheduled storyboard.

A scheduled storyboard can be trimmed only if the priority comparison object registered with this method returns <b>S_OK</b>. If the new storyboard trims the scheduled storyboard,  the scheduled storyboard can no longer affect a variable once the new storyboard begins to animate that variable.

Passing <b>NULL</b> for the <i>comparison</i> parameter causes Windows Animation to release its reference to any handler object you passed in earlier. This technique can be essential for breaking reference cycles without having to call the <a href="https://msdn.microsoft.com/3bcce52c-d29a-423c-ae76-eb88cbe8c8df">IUIAnimationManager::Shutdown</a> method.




## -see-also




<a href="https://msdn.microsoft.com/21f16c65-90aa-4b1f-93bc-8ee0488c6ded">IUIAnimationManager</a>



<a href="https://msdn.microsoft.com/cea146d1-4a9c-4089-8015-ac16602f5afd">IUIAnimationManager::SetCancelPriorityComparison</a>



<a href="https://msdn.microsoft.com/bf2a7782-3541-483e-8d5e-3e82693f103c">IUIAnimationManager::SetCompressPriorityComparison</a>



<a href="https://msdn.microsoft.com/00a3d7e4-7ad2-46a8-a9c2-0e725005c00b">IUIAnimationManager::SetConcludePriorityComparison</a>



<a href="https://msdn.microsoft.com/65311cf0-f8d4-4d2c-bd4d-585ae5d921df">IUIAnimationPriorityComparison</a>
 

 

