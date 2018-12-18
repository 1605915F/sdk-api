---
UID: NF:stralign.uaw_wcslen
title: uaw_wcslen function
author: windows-sdk-content
description: Retrieves the number of characters in a null-terminated Unicode string.
old-location: winprog\uaw_wcslen.htm
tech.root: devnotes
ms.assetid: 006e09df-9df3-48e8-9eaa-d8e95369424a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: stralign/uaw_wcslen, uaw_wcslen, uaw_wcslen function [Windows API], winprog.uaw_wcslen
ms.topic: function
req.header: stralign.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
api_name:
 - uaw_wcslen
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# uaw_wcslen function


## -description


<p class="CCE_Message">[This function is not supported and may be altered or unavailable in the future. Applications should use the <b>wcslen</b> function.]

Retrieves the number of characters in a null-terminated Unicode string.


## -parameters




### -param String [in]

A pointer to a null-terminated Unicode string.


## -returns



The return value is the number of characters in <i>String</i>, not including the terminating null character.




## -remarks



This function is available only on 64-bit Windows.



