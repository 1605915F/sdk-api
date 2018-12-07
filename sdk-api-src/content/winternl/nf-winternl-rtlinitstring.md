---
UID: NF:winternl.RtlInitString
title: RtlInitString function
author: windows-sdk-content
description: Initializes a counted string.
old-location: winprog\rtlinitstring.htm
tech.root: devnotes
ms.assetid: VS|winui|~\winui\windowsuserinterface\lowlevelclientsupport\misc\rtlinitstring.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: RtlInitString, RtlInitString function [Windows API], winprog.rtlinitstring, winternl/RtlInitString, winui.rtlinitstring
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winternl.h
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
 - RtlInitString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# RtlInitString function


## -description


Initializes a counted string.
    



## -parameters




### -param DestinationString [in, out]

The counted string to be initialized. The <i>DestinationString</i> is initialized to point to the <i>SourceString</i>. The <b>Length</b> and <b>MaximumLength</b> fields of the <i>DestinationString</i> are initialized to the length of the <i>SourceString</i>. 


### -param SourceString [in]

A pointer to a null-terminated string. If the <i>SourceString</i> is not specified, the <b>Length</b> and <b>MaximumLength</b> fields of the <i>DestinationString</i> are initialized to zero.


## -returns



This function does not return a value.




## -remarks



<b>Security Warning:  </b>Do not allow the <i>SourceString</i> parameter size to exceed <b>MAX_USHORT</b> characters.

Because there is no import library for this function, you must use <a href="https://msdn.microsoft.com/a0d7fc09-f888-4f46-a571-d3719a627597">GetProcAddress</a>.


		

<div class="alert"><b>Note</b>  <b>RtlInitString</b> is available in Windows XP. It might be altered or unavailable in subsequent versions.</div>
<div> </div>


