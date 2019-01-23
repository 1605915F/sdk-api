---
UID: NF:authz.AuthzAddSidsToContext
title: AuthzAddSidsToContext function
author: windows-sdk-content
description: Creates a copy of an existing context and appends a given set of security identifiers (SIDs) and restricted SIDs.
old-location: security\authzaddsidstocontext.htm
tech.root: SecAuthZ
ms.assetid: 4744013b-7f2e-4ebb-8944-10ffcc6006d0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AuthzAddSidsToContext, AuthzAddSidsToContext function [Security], _win32_authzaddsidstocontext, authz/AuthzAddSidsToContext, security.authzaddsidstocontext
ms.topic: function
req.header: authz.h
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
req.lib: Authz.lib
req.dll: Authz.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Authz.dll
api_name:
 - AuthzAddSidsToContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
---

# AuthzAddSidsToContext function


## -description


The <b>AuthzAddSidsToContext</b> function creates a copy of an existing context and appends a given set of <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifiers</a> (SIDs) and restricted SIDs.


## -parameters




### -param hAuthzClientContext [in]

An <b>AUTHZ_CLIENT_CONTEXT_HANDLE</b> structure to be copied as the basis for <i>NewClientContext</i>.


### -param Sids [in]

A pointer to a 
<a href="https://msdn.microsoft.com/d15d5a3f-6b38-4b92-b59c-ff0d27d111d9">SID_AND_ATTRIBUTES</a> structure containing the SIDs and attributes to be added to the unrestricted part of the client context.


### -param SidCount [in]

The number of SIDs to be added.


### -param RestrictedSids [in]

A pointer to a <a href="https://msdn.microsoft.com/d15d5a3f-6b38-4b92-b59c-ff0d27d111d9">SID_AND_ATTRIBUTES</a> structure containing the SIDs and attributes to be added to the restricted part of the client context.


### -param RestrictedSidCount [in]

Number of restricted SIDs to be added.


### -param phNewAuthzClientContext [out]

A pointer to the created <b>AUTHZ_CLIENT_CONTEXT_HANDLE</b> structure containing input values for expiration time, identifier, flags, additional SIDs and restricted SIDs.


## -returns



If the function succeeds, it returns <b>TRUE</b>.

If the function fails, it returns <b>FALSE</b>. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa375742(v=VS.85).aspx">Basic Access Control Functions</a>



<a href="https://msdn.microsoft.com/d15d5a3f-6b38-4b92-b59c-ff0d27d111d9">SID_AND_ATTRIBUTES</a>
 

 

