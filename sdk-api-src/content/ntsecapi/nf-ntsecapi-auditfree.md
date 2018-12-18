---
UID: NF:ntsecapi.AuditFree
title: AuditFree function
author: windows-sdk-content
description: Frees the memory allocated by audit functions for the specified buffer.
old-location: security\auditfree_func.htm
tech.root: secauthz
ms.assetid: 697baf9b-91c4-4a88-a190-e9f6812e08af
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AuditFree, AuditFree function [Security], ntsecapi/AuditFree, security.auditfree_func
ms.topic: function
req.header: ntsecapi.h
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
 - API-MS-Win-Security-audit-l1-1-0.dll
 - sechost.dll
 - API-MS-Win-Security-audit-l1-1-1.dll
api_name:
 - AuditFree
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# AuditFree function


## -description


The <b>AuditFree</b> function frees the memory allocated by audit functions for the specified buffer. 


## -parameters




### -param Buffer [in]

A pointer to the buffer to free.


## -returns



This function does not return a value.



