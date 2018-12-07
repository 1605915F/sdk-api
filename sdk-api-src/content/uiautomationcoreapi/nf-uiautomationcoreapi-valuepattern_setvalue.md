---
UID: NF:uiautomationcoreapi.ValuePattern_SetValue
title: ValuePattern_SetValue function
author: windows-sdk-content
description: Sets the text value of an element.
old-location: winauto\uiauto_ValuePattern_SetValueConPat.htm
tech.root: WinAuto
ms.assetid: 6233abb0-7d18-4d1f-a611-28931d874bda
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ValuePattern_SetValue, ValuePattern_SetValue function [Windows Accessibility], uiauto.uiauto_ValuePattern_SetValueConPat, uiauto_ValuePattern_SetValueConPat, uiautomationcoreapi/ValuePattern_SetValue, winauto.uiauto_ValuePattern_SetValueConPat
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: uiautomationcoreapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uiautomationcore.lib
req.dll: Uiautomationcore.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Uiautomationcore.dll
api_name:
 - ValuePattern_SetValue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ValuePattern_SetValue function


## -description


<div class="alert"><b>Note</b>  This function is deprecated. Client applications should use the Microsoft UI Automation Component Object Model (COM) interfaces instead.</div><div> </div>Sets the text value of an element.


## -parameters




### -param hobj [in]

Type: <b>HUIAPATTERNOBJECT</b>

The control pattern object.


### -param pVal [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCTSTR</a></b>

The string to set the element's content to.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns S_OK if successful or an error value otherwise.



