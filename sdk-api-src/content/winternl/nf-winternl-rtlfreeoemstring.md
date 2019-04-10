---
UID: NF:winternl.RtlFreeOemString
title: RtlFreeOemString function (winternl.h)
author: windows-sdk-content
description: Frees the string buffer allocated by RtlUnicodeStringToOemString.
old-location: winprog\rtlfreeoemstring.htm
tech.root: DevNotes
ms.assetid: VS|winui|~\winui\windowsuserinterface\lowlevelclientsupport\misc\rtlfreeoemstring.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: RtlFreeOemString, RtlFreeOemString function [Windows API], winprog.rtlfreeoemstring, winternl/RtlFreeOemString, winui.rtlfreeoemstring
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
 - RtlFreeOemString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# RtlFreeOemString function


## -description


Frees the string buffer allocated by
    <a href="https://msdn.microsoft.com/en-us/library/ms648422(v=VS.85).aspx">RtlUnicodeStringToOemString</a>.


## -parameters




### -param OemString [in, out]

Address of the OEM string whose buffer
        was previously allocated by <a href="https://msdn.microsoft.com/en-us/library/ms648422(v=VS.85).aspx">RtlUnicodeStringToOemString</a>.


## -returns



This function does not return a value.




## -remarks



This routine releases the <b>Buffer</b> member of the <a href="https://msdn.microsoft.com/en-us/library/ms648424(v=VS.85).aspx">OEM_STRING</a> structure. The <b>Length</b> and <b>MaximumLength</b> members are not affected by this routine.
		



