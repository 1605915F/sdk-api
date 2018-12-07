---
UID: NF:uiautomationclient.IUIAutomation2.put_AutoSetFocus
title: IUIAutomation2::put_AutoSetFocus
author: windows-sdk-content
description: Specifies whether calls to UI Automation control pattern methods automatically set focus to the target element.
old-location: winauto\uiauto_IUIAutomation2_AutoSetFocus.htm
tech.root: WinAuto
ms.assetid: 86B0C641-6A5B-4E1A-ADB8-7663B246739B
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AutoSetFocus property [Windows Accessibility], AutoSetFocus property [Windows Accessibility],IUIAutomation2 interface, IUIAutomation2 interface [Windows Accessibility],AutoSetFocus property, IUIAutomation2.AutoSetFocus, IUIAutomation2.put_AutoSetFocus, IUIAutomation2::AutoSetFocus, IUIAutomation2::get_AutoSetFocus, IUIAutomation2::put_AutoSetFocus, put_AutoSetFocus, uiautomationclient/IUIAutomation2::AutoSetFocus, uiautomationclient/IUIAutomation2::get_AutoSetFocus, uiautomationclient/IUIAutomation2::put_AutoSetFocus, winauto.uiauto_IUIAutomation2_AutoSetFocus
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: uiautomationclient.h
req.include-header: UIAutomation.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
req.dll: UIAutomationCore.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - UIAutomationCore.dll
api_name:
 - IUIAutomation2.AutoSetFocus
 - IUIAutomation2.get_AutoSetFocus
 - IUIAutomation2.put_AutoSetFocus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAutomation2::put_AutoSetFocus


## -description


Specifies whether calls to UI Automation control pattern methods automatically set focus to the target element.

This property is read/write.


## -parameters


## -remarks



 By default, most UI Automation methods that perform an action on an element, such as <a href="https://msdn.microsoft.com/dd04426c-edc5-4ee9-95ac-22f32fb14daa">IUIAutomationInvokePattern::Invoke</a> and <a href="https://msdn.microsoft.com/9b4caa59-bda4-4cc6-b2d8-ff47ea292746">IUIAutomationValuePattern::SetValue</a>, set focus to the element before performing the action. For most applications, setting the focus results in a more consistent user experience.  In situations where setting the focus would be disruptive, such as automating a drop-down menu, you can set <b>AutoSetFocus</b> to FALSE to prevent UI Automation methods from setting the focus. 




## -see-also




<a href="https://msdn.microsoft.com/45B4D41E-9C5C-47C7-86EB-D7B9BA14211B">IUIAutomation2</a>
 

 

