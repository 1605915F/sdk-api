---
UID: NF:uiautomationclient.IUIAutomationExpandCollapsePattern.Collapse
title: IUIAutomationExpandCollapsePattern::Collapse
author: windows-sdk-content
description: Hides all child nodes, controls, or content of the element.
old-location: winauto\uiauto_IUIAutomationExpandCollapsePattern_Collapse.htm
tech.root: WinAuto
ms.assetid: 9337d2dd-08db-4af7-ad65-e113811dd7ba
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Collapse, Collapse method [Windows Accessibility], Collapse method [Windows Accessibility],IUIAutomationExpandCollapsePattern interface, IUIAutomationExpandCollapsePattern interface [Windows Accessibility],Collapse method, IUIAutomationExpandCollapsePattern.Collapse, IUIAutomationExpandCollapsePattern::Collapse, uiauto.uiauto_IUIAutomationExpandCollapsePattern_Collapse, uiauto_IUIAutomationExpandCollapsePattern_Collapse, uiautomationclient/IUIAutomationExpandCollapsePattern::Collapse, winauto.uiauto_IUIAutomationExpandCollapsePattern_Collapse
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: uiautomationclient.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista, Windows XP with SP3 and Platform Update for Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008, Windows Server 2003 with SP2 and Platform Update for Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: UIAutomationClient.idl
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
 - UIAutomationClient.h
api_name:
 - IUIAutomationExpandCollapsePattern.Collapse
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAutomationExpandCollapsePattern::Collapse


## -description


Hides all child nodes, controls, or content of the element.


## -parameters






## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This is a blocking method that returns after the element has been collapsed.

There are cases when a element that is marked as a leaf node might not know whether it has children until either the <b>IUIAutomationExpandCollapsePattern::Collapse</b> or the <a href="https://msdn.microsoft.com/bc21cffc-63fe-4c5d-9c4d-35e1bab67a7c">IUIAutomationExpandCollapsePattern::Expand</a> method is called. This behavior is possible with a tree view control that does delayed loading of its child items. For example, Microsoft Windows Explorer might display the expand icon for a node even though there are currently no child items; when the icon is clicked, the control polls for child items, finds none, and removes the expand icon. In these cases clients should listen for a property-changed event on the <a href="https://msdn.microsoft.com/abd21a19-c7a0-44db-ad5b-64c476efa400">IUIAutomationExpandCollapsePattern::CurrentExpandCollapseState</a> property.




## -see-also




<a href="https://msdn.microsoft.com/816c28a9-2486-403e-bfbd-94d040d0aac5">IUIAutomationExpandCollapsePattern</a>
 

 

