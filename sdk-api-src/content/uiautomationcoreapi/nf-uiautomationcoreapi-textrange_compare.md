---
UID: NF:uiautomationcoreapi.TextRange_Compare
title: TextRange_Compare function (uiautomationcoreapi.h)
author: windows-sdk-content
description: Compares two text ranges.
old-location: winauto\uiauto_TextRange_CompareConPat.htm
tech.root: WinAuto
ms.assetid: 891166a2-dee6-44c9-b26c-8d1d39de72ef
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: TextRange_Compare, TextRange_Compare function [Windows Accessibility], uiauto.uiauto_TextRange_CompareConPat, uiauto_TextRange_CompareConPat, uiautomationcoreapi/TextRange_Compare, winauto.uiauto_TextRange_CompareConPat
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
 - TextRange_Compare
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# TextRange_Compare function


## -description


<div class="alert"><b>Note</b>  This function is deprecated. Client applications should use the Microsoft UI Automation Component Object Model (COM) interfaces instead.</div><div> </div>Compares two text ranges.


## -parameters




### -param hobj [in]

Type: <b>HUIATEXTRANGE</b>

The first text range to compare.


### -param range [in]

Type: <b>HUIATEXTRANGE</b>

The second text range to compare.


### -param pRetVal [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a>*</b>

When this function returns, contains <b>TRUE</b> if the two objects span the same text; otherwise <b>FALSE</b>. 
				This parameter is passed uninitialized.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

Returns S_OK if successful or an error value otherwise.



