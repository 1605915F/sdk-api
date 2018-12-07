---
UID: NF:werapi.WerUnregisterAdditionalProcess
title: WerUnregisterAdditionalProcess function
author: windows-sdk-content
description: Removes a process from the list of additional processes to be included in the error report.
old-location: wer\werunregisteradditionalprocess.htm
tech.root: wer
ms.assetid: CE840EE8-5EB6-4F0F-935E-5DA9097E950F
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WerUnregisterAdditionalProcess, WerUnregisterAdditionalProcess function [Windows Error Reporting], wer.werunregisteradditionalprocess, werapi/WerUnregisterAdditionalProcess
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: werapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1703 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2016 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
 - API-MS-Win-Core-Windowserrorreporting-l1-1-0.dll
 - KernelBase.dll
api_name:
 - WerUnregisterAdditionalProcess
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WerUnregisterAdditionalProcess function


## -description


Removes a process from the list of additional processes to be included in the error report.


## -parameters




### -param processId

The Id of the process to remove. It must have been previously registered with <a href="https://msdn.microsoft.com/F4E44C22-6BE1-4512-80F6-1B6741E3ADBB">WerRegisterAdditionalProcess</a>.


## -returns



This function returns <b>S_OK</b> on success or an error code on failure, including the following error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WER_E_INVALID_STATE</b></dt>
</dl>
</td>
<td width="60%">
The process state is not valid. For example, the process is in <a href="https://msdn.microsoft.com/9357786c-1992-4e28-ac75-c2dfda1df7f1">application recovery mode</a>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WER_E_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The list of registered processes does not contain the specified process.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/4e28f379-5793-4d76-898e-d87a0291c034">WER Functions</a>



<a href="https://msdn.microsoft.com/F4E44C22-6BE1-4512-80F6-1B6741E3ADBB">WerRegisterAdditionalProcess</a>



<a href="https://msdn.microsoft.com/5c076588-779c-4cd2-9fd9-1db3039e37a2">Windows Error Reporting</a>
 

 

