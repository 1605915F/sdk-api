---
UID: NF:uianimation.IUIAnimationManagerEventHandler2.OnManagerStatusChanged
title: IUIAnimationManagerEventHandler2::OnManagerStatusChanged (uianimation.h)
author: windows-sdk-content
description: Handles status changes to an animation manager.
old-location: uianimation\iuianimationmanagereventhandler2_onmanagerstatuschanged.htm
tech.root: UIAnimation
ms.assetid: 398A52B3-E7FA-466E-BCED-0A6E91633CF7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUIAnimationManagerEventHandler2 interface [Windows Animation],OnManagerStatusChanged method, IUIAnimationManagerEventHandler2.OnManagerStatusChanged, IUIAnimationManagerEventHandler2::OnManagerStatusChanged, OnManagerStatusChanged, OnManagerStatusChanged method [Windows Animation], OnManagerStatusChanged method [Windows Animation],IUIAnimationManagerEventHandler2 interface, uianimation.iuianimationmanagereventhandler2_onmanagerstatuschanged, uianimation/IUIAnimationManagerEventHandler2::OnManagerStatusChanged
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
 - IUIAnimationManagerEventHandler2.OnManagerStatusChanged
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAnimationManagerEventHandler2::OnManagerStatusChanged


## -description


Handles status changes to an <a href="https://msdn.microsoft.com/BD7DAD23-2A7D-4EE7-9BCF-8380F928674D">animation manager</a>.


## -parameters




### -param newStatus [in]

The new status of the animation manager.


### -param previousStatus [in]

The previous status of the animation manager.


## -returns



If the method succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/38f15d61-d415-4c7d-b454-5144fc7c9b1e">Windows Animation Error Codes</a> for a list of error codes.




## -remarks



Calls made to other Windows Animation methods from <b>IUIAnimationManager2::OnManagerStatusChanged</b> fail and return <b>UI_E_ILLEGAL_REENTRANCY</b>.




## -see-also




<a href="https://msdn.microsoft.com/E989CED1-C6B7-4086-944E-924836AA7ECB">IUIAnimationManager2::GetStatus</a>



<a href="https://msdn.microsoft.com/3D3DAC6C-6904-4962-BB17-18FA97678834">IUIAnimationManagerEventHandler2</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd317043(v=VS.85).aspx">UI_ANIMATION_MANAGER_STATUS</a>
 

 

