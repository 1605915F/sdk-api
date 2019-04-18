---
UID: NF:uiautomationcoreapi.UiaNodeFromProvider
title: UiaNodeFromProvider function (uiautomationcoreapi.h)
author: windows-sdk-content
description: Retrieves the UI Automation node for a raw element provider.
old-location: winauto\uiauto_UiaNodeFromProviderFunction.htm
tech.root: WinAuto
ms.assetid: 9f280fbb-ad14-43ea-bc1e-a281987c5898
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: UiaNodeFromProvider, UiaNodeFromProvider function [Windows Accessibility], uiauto.uiauto_UiaNodeFromProviderFunction, uiauto_UiaNodeFromProviderFunction, uiautomationcoreapi/UiaNodeFromProvider, winauto.uiauto_UiaNodeFromProviderFunction
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
 - UiaNodeFromProvider
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# UiaNodeFromProvider function


## -description


<div class="alert"><b>Note</b>  This function is deprecated. Client applications should use the Microsoft UI Automation Component Object Model (COM) interfaces instead.</div><div> </div>Retrieves the UI Automation node for a raw element provider.


## -parameters




### -param pProvider [in]

Type: <b><a href="https://msdn.microsoft.com/f0ec6185-acd0-4df7-88f4-fd00747f98bf">IRawElementProviderSimple</a>*</b>

The address of the <a href="https://msdn.microsoft.com/f0ec6185-acd0-4df7-88f4-fd00747f98bf">IRawElementProviderSimple</a> interface of the provider.


### -param phnode [out]

Type: <b>HUIANODE*</b>

The address of a variable that receives the UI Automation node for the raw element provider.
				This parameter is passed uninitialized.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns S_OK if successful or an error value otherwise.



