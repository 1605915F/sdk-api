---
UID: NF:winternl.RtlFreeAnsiString
title: RtlFreeAnsiString function (winternl.h)
author: windows-sdk-content
description: Frees the string buffer allocated by RtlUnicodeStringToAnsiString.
old-location: winprog\rtlfreeansistring.htm
tech.root: DevNotes
ms.assetid: VS|winui|~\winui\windowsuserinterface\lowlevelclientsupport\misc\rtlfreeansistring.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: RtlFreeAnsiString, RtlFreeAnsiString function [Windows API], winprog.rtlfreeansistring, winternl/RtlFreeAnsiString, winui.rtlfreeansistring
ms.topic: function
req.header: winternl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
req.dll: Ntdll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Ntdll.dll
api_name:
 - RtlFreeAnsiString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# RtlFreeAnsiString function


## -description


Frees the string buffer allocated by <a href="https://msdn.microsoft.com/en-us/library/ms648421(v=VS.85).aspx">RtlUnicodeStringToAnsiString</a>.


## -parameters




### -param AnsiString [in]

A pointer to an ANSI string whose buffer was previously allocated by <a href="https://msdn.microsoft.com/en-us/library/ms648421(v=VS.85).aspx">RtlUnicodeStringToAnsiString</a>.


## -returns



This function does not return a value.




## -remarks



This routine does not release the Unicode string buffer passed to <a href="https://msdn.microsoft.com/en-us/library/ms648421(v=VS.85).aspx">RtlUnicodeStringToAnsiString</a>.



