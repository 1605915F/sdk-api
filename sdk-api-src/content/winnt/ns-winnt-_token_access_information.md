---
UID: NS:winnt._TOKEN_ACCESS_INFORMATION
title: "_TOKEN_ACCESS_INFORMATION"
author: windows-sdk-content
description: Specifies all the information in a token that is necessary to perform an access check.
old-location: security\token_access_information.htm
tech.root: secauthz
ms.assetid: cb727b91-c88f-48f3-8329-020d3f727dc7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PTOKEN_ACCESS_INFORMATION, PTOKEN_ACCESS_INFORMATION, PTOKEN_ACCESS_INFORMATION structure pointer [Security], TOKEN_ACCESS_INFORMATION, TOKEN_ACCESS_INFORMATION structure [Security], _TOKEN_ACCESS_INFORMATION, security.token_access_information, winnt/PTOKEN_ACCESS_INFORMATION, winnt/TOKEN_ACCESS_INFORMATION"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winnt.h
req.include-header: Windows.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Winnt.h
api_name:
 - TOKEN_ACCESS_INFORMATION
product: Windows
targetos: Windows
req.typenames: TOKEN_ACCESS_INFORMATION, *PTOKEN_ACCESS_INFORMATION
req.redist: 
---

# _TOKEN_ACCESS_INFORMATION structure


## -description


The <b>TOKEN_ACCESS_INFORMATION</b> structure specifies all the information in a token that is necessary to perform an access check.<div class="alert"><b>Note</b>  This structure doesn't contain token claim information. Applications that support conditional expression <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">access control entries</a> (ACEs) should not use this structure for verifying access. For information about access validation support for conditional expressions, see the <a href="https://msdn.microsoft.com/633c2a73-169c-4e0c-abb6-96c360bd63cf">AuthzAccessCheck</a> and <a href="https://msdn.microsoft.com/c2d144f4-9eeb-4723-9d28-97cfd1a07274">AccessCheckAndAuditAlarm</a> functions.</div>
<div> </div>



## -struct-fields




### -field SidHash

A pointer to a <a href="https://msdn.microsoft.com/ef6e32f5-b47e-463e-a447-bed149b8d616">SID_AND_ATTRIBUTES_HASH</a> structure that specifies a hash of the token's <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifier</a> (SID).


### -field RestrictedSidHash

A pointer to a <a href="https://msdn.microsoft.com/ef6e32f5-b47e-463e-a447-bed149b8d616">SID_AND_ATTRIBUTES_HASH</a> structure that specifies a hash of the token's restricted SID.


### -field Privileges

A pointer to a <a href="https://msdn.microsoft.com/c9016511-740f-44f3-92ed-17cc518c6612">TOKEN_PRIVILEGES</a> structure that specifies information about the token's privileges.


### -field AuthenticationId

A <a href="https://msdn.microsoft.com/a812a46b-f23f-45b1-a6c6-48f931b78750">LUID</a> structure that specifies the token's identity.


### -field TokenType

A value of the <a href="https://msdn.microsoft.com/51b6717e-3fda-4af4-8995-4ac571eae2fd">TOKEN_TYPE</a> enumeration that specifies the token's type.


### -field ImpersonationLevel

A value of the <a href="https://msdn.microsoft.com/a75ad777-c88e-4899-be50-0118c113a600">SECURITY_IMPERSONATION_LEVEL</a> enumeration that specifies the token's impersonation level.


### -field MandatoryPolicy

A <a href="https://msdn.microsoft.com/f5fc438b-c4f0-46f6-a188-52ce660d13da">TOKEN_MANDATORY_POLICY</a> structure that specifies the token's mandatory integrity policy.


### -field Flags

Reserved. Must be set to zero.


### -field AppContainerNumber

The app container number for the token or zero if this is not an app container token.

<b>Windows Server 2008 R2, Windows 7, Windows Server 2008 and Windows Vista:  </b>This member is not available.


### -field PackageSid

The app container SID or <b>NULL</b> if this is not an app container token.

<b>Windows Server 2008 R2, Windows 7, Windows Server 2008 and Windows Vista:  </b>This member is not available.


### -field CapabilitiesHash

Pointer to a <a href="https://msdn.microsoft.com/ef6e32f5-b47e-463e-a447-bed149b8d616">SID_AND_ATTRIBUTES_HASH</a> structure that specifies a hash of the token's capability SIDs.

<b>Windows Server 2008 R2, Windows 7, Windows Server 2008 and Windows Vista:  </b>This member is not available.


### -field TrustLevelSid

The protected process trust level of the token.


### -field SecurityAttributes

Reserved. Must be set to <b>NULL</b>.

<b>Prior to Windows 10:  </b>This member is not available.


## -see-also




<a href="https://msdn.microsoft.com/cb606665-1266-4e71-a145-9b04bf157cdc">TOKEN_INFORMATION_CLASS</a>
 

 

