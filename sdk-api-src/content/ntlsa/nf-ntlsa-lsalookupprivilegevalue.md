---
UID: NF:ntlsa.LsaLookupPrivilegeValue
title: LsaLookupPrivilegeValue function (ntlsa.h)
author: windows-sdk-content
description: Retrieves the locally unique identifier (LUID) used by the Local Security Authority (LSA) to represent the specified privilege name.
old-location: security\lsalookupprivilegevalue.htm
tech.root: SecMgmt
ms.assetid: 4926fff9-6e1a-475c-95ab-78c9b67aaa87
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: LsaLookupPrivilegeValue, LsaLookupPrivilegeValue function [Security], ntlsa/LsaLookupPrivilegeValue, security.lsalookupprivilegevalue
ms.topic: function
req.header: ntlsa.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Advapi32.lib
req.dll: Advapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Advapi32.dll
api_name:
 - LsaLookupPrivilegeValue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# LsaLookupPrivilegeValue function


## -description


Retrieves the <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">locally unique identifier</a> (LUID) used by the <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">Local Security Authority</a> (LSA) to  represent the specified privilege name.

This function is not declared in a public header.

Do not use this function. Instead, use <a href="https://msdn.microsoft.com/334b8ba8-101d-43a1-a8bf-1c7e0448c272">LookupPrivilegeValue</a>.


## -parameters




### -param PolicyHandle

A handle to the LSA <a href="https://msdn.microsoft.com/4253c7fb-85f5-441d-90bf-492e802ad0f8">Policy</a> object.


### -param Name

A pointer to a null-terminated string that specifies the name of the privilege, as defined in the Winnt.h header file.


### -param Value

A pointer to a variable that receives the LUID by which the privilege is known by the LSA.


## -returns



If the function succeeds, return <b>STATUS_SUCCESS</b>.

If the function fails, return an <b>NTSTATUS</b> code that indicates the reason it failed.



