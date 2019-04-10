---
UID: NF:uiautomationcore.ISelectionProvider.GetSelection
title: ISelectionProvider::GetSelection (uiautomationcore.h)
author: windows-sdk-content
description: Retrieves a Microsoft UI Automation provider for each child element that is selected.
old-location: winauto\uiauto_ISelectionProvider_GetSelection.htm
tech.root: WinAuto
ms.assetid: f97481b9-f227-47fb-9163-a65a259c9d78
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetSelection, GetSelection method [Windows Accessibility], GetSelection method [Windows Accessibility],ISelectionProvider interface, ISelectionProvider interface [Windows Accessibility],GetSelection method, ISelectionProvider.GetSelection, ISelectionProvider::GetSelection, uiauto.uiauto_ISelectionProvider_GetSelection, uiauto_ISelectionProvider_GetSelection, uiautomationcore/ISelectionProvider::GetSelection, winauto.uiauto_ISelectionProvider_GetSelection
ms.topic: method
req.header: uiautomationcore.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAutomationCore.idl
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
 - UIAutomationCore.h
api_name:
 - ISelectionProvider.GetSelection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ISelectionProvider::GetSelection


## -description


Retrieves a Microsoft UI Automation provider for each child element that is selected.
        


## -parameters




### -param pRetVal [out, retval]

Type: <b><a href="https://go.microsoft.com/fwlink/p/?linkid=180754">SAFEARRAY</a>**</b>

Receives a pointer to a <a href="https://go.microsoft.com/fwlink/p/?linkid=180754">SAFEARRAY</a> that contains an array of pointers to the <a href="https://msdn.microsoft.com/f0ec6185-acd0-4df7-88f4-fd00747f98bf">IRawElementProviderSimple</a> interfaces
				of the selected elements. This parameter is passed uninitialized.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/07e87cfd-d565-41b5-a68d-b99dd191fa95">Best Practices for Using Safe Arrays</a>



<b>Conceptual</b>



<a href="https://msdn.microsoft.com/e02731f8-e58d-4c66-95bf-005cf954471c">ISelectionProvider</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/8928c889-0e0a-439f-87e8-a9d121fcf73f">UI Automation Providers Overview</a>
 

 

