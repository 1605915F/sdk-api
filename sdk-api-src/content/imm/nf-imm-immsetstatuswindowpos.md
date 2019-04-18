---
UID: NF:imm.ImmSetStatusWindowPos
title: ImmSetStatusWindowPos function (imm.h)
author: windows-sdk-content
description: Sets the position of the status window.
old-location: intl\immsetstatuswindowpos.htm
tech.root: Intl
ms.assetid: 36a3251a-0d8b-404b-8839-e0724b251cd1
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ImmSetStatusWindowPos, ImmSetStatusWindowPos function [Internationalization for Windows Applications], _win32_ImmSetStatusWindowPos, imm/ImmSetStatusWindowPos, intl.immsetstatuswindowpos
ms.topic: function
req.header: imm.h
req.include-header: Immdev.h, Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only],East Asian language support installed.
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
req.lib: Imm32.lib
req.dll: Imm32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Imm32.dll
api_name:
 - ImmSetStatusWindowPos
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ImmSetStatusWindowPos function


## -description


Sets the position of the status window.


## -parameters




### -param HIMC [in]

Handle to the input context.


### -param lpptPos [in]

Pointer to a <a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a> structure containing the new position of the status window, in screen coordinates relative to the upper left corner of the display screen.


## -returns



Returns a nonzero value if successful, or 0 otherwise.




## -remarks



This function causes an <a href="https://msdn.microsoft.com/15e65aff-67d9-4d1a-a6a7-b921cecb3aec">IMN_SETSTATUSWINDOWPOS</a> command to be sent to the application.




## -see-also




<a href="https://msdn.microsoft.com/15e65aff-67d9-4d1a-a6a7-b921cecb3aec">IMN_SETSTATUSWINDOWPOS</a>



<a href="https://msdn.microsoft.com/3e23e004-514a-4021-bd20-5ac55547258f">Input Method Manager</a>



<a href="https://msdn.microsoft.com/833c07eb-0ecf-41e2-9e01-8d83e51ffcef">Input Method Manager Functions</a>
 

 

