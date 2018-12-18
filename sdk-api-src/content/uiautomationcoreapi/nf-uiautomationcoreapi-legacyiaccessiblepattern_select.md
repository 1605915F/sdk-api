---
UID: NF:uiautomationcoreapi.LegacyIAccessiblePattern_Select
title: LegacyIAccessiblePattern_Select function
author: windows-sdk-content
description: Performs a Microsoft Active Accessibility selection.
old-location: winauto\uiauto_LegacyIAccessiblePattern_Select.htm
tech.root: WinAuto
ms.assetid: 34235a9b-e4e2-4766-ab99-2b71cf0797d0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: LegacyIAccessiblePattern_Select, LegacyIAccessiblePattern_Select function [Windows Accessibility], uiauto.uiauto_LegacyIAccessiblePattern_Select, uiauto_LegacyIAccessiblePattern_Select, uiautomationcoreapi/LegacyIAccessiblePattern_Select, winauto.uiauto_LegacyIAccessiblePattern_Select
ms.topic: function
req.header: uiautomationcoreapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista, Windows XP with SP3 and Platform Update for Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008, Windows Server 2003 with SP2 and Platform Update for Windows Server 2008 [desktop apps only]
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
 - LegacyIAccessiblePattern_Select
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# LegacyIAccessiblePattern_Select function


## -description


<div class="alert"><b>Note</b>  This function is deprecated. Client applications should use the Microsoft UI Automation Component Object Model (COM) interfaces instead.</div><div> </div>Performs a Microsoft Active Accessibility selection.


## -parameters




### -param hobj [in]

Type: <b>HUIAPATTERNOBJECT</b>

The <i>control pattern</i> object.


### -param flagsSelect [in]

Type: <b>long</b>

Specifies which selection or focus operations are to be performed. This parameter must have a combination of the values described in <a href="https://msdn.microsoft.com/52755540-dcf4-4e0b-bb5c-88b05f134d79">SELFLAG Constants</a>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns S_OK if successful or an error value otherwise.



