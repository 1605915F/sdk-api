---
UID: NS:sspi._SECURITY_STRING
title: SECURITY_STRING
author: windows-sdk-content
description: Used as the string interface for kernel operations and is a clone of the UNICODE_STRING structure.
old-location: security\security_string.htm
tech.root: secauthn
ms.assetid: 4E03761C-8199-4D9F-B9DA-8941F0CC6700
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSECURITY_STRING, PSECURITY_STRING, PSECURITY_STRING structure pointer [Security], SECURITY_STRING, SECURITY_STRING structure [Security], security.security_string, sspi/PSECURITY_STRING, sspi/SECURITY_STRING"
ms.topic: struct
req.header: sspi.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Sspi.h
api_name:
 - SECURITY_STRING
product: Windows
targetos: Windows
req.typenames: SECURITY_STRING, *PSECURITY_STRING
req.redist: 
---

# SECURITY_STRING structure


## -description


The <b>SECURITY_STRING</b> structure is used as the string interface for kernel operations and is a clone of the <a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> structure. This is used for 32-bit mode.


## -struct-fields




### -field Length

Specifies the length, in bytes, of the string pointed to by the <b>Buffer</b> member, not including the terminating <b>NULL</b> character, if any.


### -field MaximumLength

Specifies the total size, in bytes, of memory allocated for <b>Buffer</b>. Up to <b>MaximumLength</b> bytes may be written into the buffer without trampling memory.


### -field Buffer

Pointer to a wide-character string. Note that the strings returned by the various LSA functions might not be <b>null</b>-terminated.


### -field Buffer.size_is

 


### -field Buffer.size_is.MaximumLength/2

 


### -field Buffer.length_is

 


### -field Buffer.length_is.Length/2

 



