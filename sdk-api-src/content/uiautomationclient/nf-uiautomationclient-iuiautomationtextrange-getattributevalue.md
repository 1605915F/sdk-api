---
UID: NF:uiautomationclient.IUIAutomationTextRange.GetAttributeValue
title: IUIAutomationTextRange::GetAttributeValue (uiautomationclient.h)
author: windows-sdk-content
description: Retrieves the value of the specified text attribute across the entire text range.
old-location: winauto\uiauto_IUIAutomationTextRange_GetAttributeValue.htm
tech.root: WinAuto
ms.assetid: 7a77774e-7be0-473e-a0c9-e1aa108549e1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetAttributeValue, GetAttributeValue method [Windows Accessibility], GetAttributeValue method [Windows Accessibility],IUIAutomationTextRange interface, IUIAutomationTextRange interface [Windows Accessibility],GetAttributeValue method, IUIAutomationTextRange.GetAttributeValue, IUIAutomationTextRange::GetAttributeValue, uiauto.uiauto_IUIAutomationTextRange_GetAttributeValue, uiauto_IUIAutomationTextRange_GetAttributeValue, uiautomationclient/IUIAutomationTextRange::GetAttributeValue, winauto.uiauto_IUIAutomationTextRange_GetAttributeValue
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
 - IUIAutomationTextRange.GetAttributeValue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUIAutomationTextRange::GetAttributeValue


## -description


Retrieves the value of the specified text attribute across the entire text range.


## -parameters




### -param attr [in]

Type: <b>TEXTATTRIBUTEID</b>

The identifier of the text attribute. For a list of text attribute IDs, see <a href="https://msdn.microsoft.com/67d86817-6a3f-4047-88d9-34f33f52a563">Text Attribute Identifiers</a>.


### -param value [out, retval]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/oaidl/ns-oaidl-tagvariant">VARIANT</a>*</b>

Receives the value of the specified attribute. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The type of value retrieved by this method depends on the <i>attr</i> parameter. 
For example, calling <b>GetAttributeValue</b> with the <i>attr</i> parameter set to <a href="https://msdn.microsoft.com/en-us/library/Ee671662(v=VS.85).aspx">UIA_FontNameAttributeId</a> returns a string that represents the font name of the text range,  while calling <b>GetAttributeValue</b> with <i>attr</i> set to <a href="https://msdn.microsoft.com/en-us/library/Ee671662(v=VS.85).aspx">UIA_IsItalicAttributeId</a> would return a boolean.





If the attribute specified by <i>attr</i> is not supported, the <i>value</i> parameter receives a value that is equivalent to the  <a href="https://msdn.microsoft.com/00162b3c-fab8-4559-83c0-d8c6731441c3">IUIAutomation::ReservedNotSupportedValue</a> property. 

A text range can include more than one value for a particular attribute. For example, if a text range includes more than one font, the FontName attribute will have multiple values. An attribute with more than one value is called a  <i>mixed attribute</i>.  You can determine if a particular attribute is    a mixed attribute by comparing the value retrieved from <b>GetAttributeValue</b> with the  <a href="https://msdn.microsoft.com/5b225507-deee-4f2c-a17b-f0e96963a1d0">UIAutomation::ReservedMixedAttributeValue</a> property.

The <b>GetAttributeValue</b> method retrieves the attribute value regardless of whether the text is hidden or visible.
            Use UIA_ IsHiddenAttributeId to check text visibility.




## -see-also




<a href="https://msdn.microsoft.com/1037919d-c8df-4d46-b3ce-62ee23c92145">IUIAutomationTextRange</a>



<a href="https://msdn.microsoft.com/98a82ff8-f4b9-4f62-ae69-31a2c18de70e">UI Automation Support for Textual Content</a>
 

 

