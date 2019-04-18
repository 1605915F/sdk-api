---
UID: NF:uianimation.IUIAnimationVariable2.SetTag
title: IUIAnimationVariable2::SetTag (uianimation.h)
author: windows-sdk-content
description: Sets the tag of the animation variable.
old-location: uianimation\iuianimationvariable2_settag.htm
tech.root: UIAnimation
ms.assetid: 21BAFF23-8866-432F-BB9A-0328CE0E6021
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IUIAnimationVariable2 interface [Windows Animation],SetTag method, IUIAnimationVariable2.SetTag, IUIAnimationVariable2::SetTag, SetTag, SetTag method [Windows Animation], SetTag method [Windows Animation],IUIAnimationVariable2 interface, uianimation.iuianimationvariable2_settag, uianimation/IUIAnimationVariable2::SetTag
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
 - IUIAnimationVariable2.SetTag
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IUIAnimationVariable2::SetTag


## -description


Sets the tag of the animation variable.




## -parameters




### -param object [in, optional]

The object portion of the tag. This parameter can be <b>NULL</b>.




### -param id [in]

The identifier portion of the tag.




## -returns



Returns <b>S_OK</b> if successful; otherwise an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.




## -remarks



A tag is a pairing of an integer identifier (<i>id</i>) with a COM object (<i>object</i>), and it can be used by an application to identify an animation variable.          
         Because <b>NULL</b> is a valid object component of a tag, the <i>object</i> parameter can be <b>NULL</b>.




## -see-also




<a href="https://msdn.microsoft.com/ED367DB7-91D6-4D2E-BDAB-27FA4340F091">IUIAnimationManager2::GetVariableFromTag</a>



<a href="https://msdn.microsoft.com/A676EF27-B59D-4D2D-AD5B-8F46EE337E69">IUIAnimationVariable2</a>



<a href="https://msdn.microsoft.com/29E6CA4D-527D-4C9D-9E28-2E2C67516126">IUIAnimationVariable2::GetTag</a>
 

 

