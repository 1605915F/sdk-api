---
UID: NC:ntsecpkg.LSA_AUDIT_LOGON
title: LSA_AUDIT_LOGON (ntsecpkg.h)
author: windows-sdk-content
description: The AuditLogon function is used to audit a logon attempt.
old-location: security\auditlogon.htm
tech.root: SecAuthN
ms.assetid: 1b0316ae-0c09-4a7e-8443-e59b4db9e825
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AuditLogon, AuditLogon callback function [Security], LSA_AUDIT_LOGON, LSA_AUDIT_LOGON callback, _ssp_auditlogon, ntsecpkg/AuditLogon, security.auditlogon
ms.topic: callback
req.header: ntsecpkg.h
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
 - UserDefined
api_location:
 - Ntsecpkg.h
api_name:
 - AuditLogon
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# LSA_AUDIT_LOGON callback function


## -description


The <b>AuditLogon</b> function is used to audit a logon attempt.


## -parameters




### -param Status [in]

Status of the logon attempt.


### -param SubStatus [in]

Additional status information for the logon attempt.


### -param AccountName [in]

Pointer to a 
<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a>  that contains the account name used in the logon attempt.


### -param AuthenticatingAuthority [in]

Pointer to a <a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a>  that contains the name of the authority that authenticated the logon, normally the operating system domain name.


### -param WorkstationName [in]

Pointer to a 
<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a>  that contains the name of the workstation used to attempt the logon.


### -param UserSid [in, optional]

Pointer to the SID of the <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security principal</a> attempting to logon.


### -param LogonType [in]

A 
<a href="https://msdn.microsoft.com/d775d782-9403-47b2-bb43-8f677db49eb9">SECURITY_LOGON_TYPE</a> value indicating the type of logon.


### -param TokenSource [in]

Pointer to a 
<a href="https://msdn.microsoft.com/9c533327-e4a0-4852-828c-622d190b7d1e">TOKEN_SOURCE</a> structure  that specifies the source for the user token. This value must include the package name.


### -param LogonId [in]

Pointer to the <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">logon session identifier</a>. <i>LogonId</i> is valid only if the logon attempt was successful.


## -returns



This function does not return a value.




## -remarks



A pointer to the <b>AuditLogon</b> function is available in the 
<a href="https://msdn.microsoft.com/85f04072-8634-454a-9038-737d86c5597d">LSA_SECPKG_FUNCTION_TABLE</a> structure received by the 
<a href="https://msdn.microsoft.com/d93bafc6-d946-4214-b3c0-5e5a8e359638">SpInitialize</a> function.




## -see-also




<a href="https://msdn.microsoft.com/85f04072-8634-454a-9038-737d86c5597d">LSA_SECPKG_FUNCTION_TABLE</a>



<a href="https://msdn.microsoft.com/d93bafc6-d946-4214-b3c0-5e5a8e359638">SpInitialize</a>
 

 

