---
UID: NS:ntsecpkg._LSA_TOKEN_INFORMATION_V3
title: LSA_TOKEN_INFORMATION_V3
author: windows-sdk-content
description: Adds claim support to the LSA token and contains information an authentication package can place in a Version 3 Windows token object and has superceded LSA_TOKEN_INFORMATION_V1.
old-location: security\lsa_token_information_v3.htm
tech.root: secauthn
ms.assetid: 927828CD-9763-4CE4-B3E7-376181EA7C70
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PLSA_TOKEN_INFORMATION_V3, LSA_TOKEN_INFORMATION_V3, LSA_TOKEN_INFORMATION_V3 structure [Security], PLSA_TOKEN_INFORMATION_V3, PLSA_TOKEN_INFORMATION_V3 structure pointer [Security], _LSA_TOKEN_INFORMATION_V3, ntsecpkg/LSA_TOKEN_INFORMATION_V3, ntsecpkg/PLSA_TOKEN_INFORMATION_V3, security.lsa_token_information_v3"
ms.topic: struct
req.header: ntsecpkg.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - Ntsecpkg.h
api_name:
 - LSA_TOKEN_INFORMATION_V3
product: Windows
targetos: Windows
req.typenames: LSA_TOKEN_INFORMATION_V3, *PLSA_TOKEN_INFORMATION_V3
req.redist: 
---

# LSA_TOKEN_INFORMATION_V3 structure


## -description


The <b>LSA_TOKEN_INFORMATION_V3</b> structure adds claim support to the LSA token and contains information an <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">authentication package</a> can place in a Version 3 Windows token object and has superceded <a href="https://msdn.microsoft.com/e4c43828-aa5c-443c-93ad-96bb986533c5">LSA_TOKEN_INFORMATION_V1</a>.

A Version 3 Windows token object stores all the information needed to build a token from the authentication package to the <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">Local Security Authority</a> (LSA). The LSA passes this information into the kernel to create a token object and to return a handle to that token object to the caller of <a href="https://msdn.microsoft.com/75968d53-5af2-4d77-9486-26403b73c954">LsaLogonUser</a>. LSA assumes that the first member of this structure are identical to those in the <a href="https://msdn.microsoft.com/e4c43828-aa5c-443c-93ad-96bb986533c5">LSA_TOKEN_INFORMATION_V1</a> structure.


## -struct-fields




### -field ExpirationTime

Time at which the <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security context</a> becomes not valid. Use a value in the distant future if the context never expires. The current version of the operating system kernel does not enforce this expiration time.


### -field User


<a href="https://msdn.microsoft.com/5dd8172d-7b1a-4cc0-b667-5fe91d278393">TOKEN_USER</a> structure that contains the SID of the user logging on. The <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifier</a> SID value is in a separately allocated block of memory.


### -field Groups


<a href="https://msdn.microsoft.com/387dd7f8-4177-40fa-b5fd-bb4b371a0e64">TOKEN_GROUPS</a> structure that contains the SIDs of groups the user is a member of. This should not include WORLD or other system-defined and system-assigned SIDs. These will be added automatically by the LSA. 




Each SID is expected to be in a separately allocated block of memory. The <a href="https://msdn.microsoft.com/387dd7f8-4177-40fa-b5fd-bb4b371a0e64">TOKEN_GROUPS</a> structure is also expected to be in a separately allocated block of memory. All of these memory blocks should be allocated by calling the <a href="https://msdn.microsoft.com/956e7aaf-e8b3-4db5-945a-b579f946b769">AllocatePrivateHeap</a> function.


### -field PrimaryGroup


<a href="https://msdn.microsoft.com/d23ebe6c-36a3-434a-a0fa-fcdf50dd19a0">TOKEN_PRIMARY_GROUP</a> structure that is used to establish the primary group of the user. This value does not have to correspond to one of the SIDs assigned to the user. 




The SID pointed to by this structure is expected to be in a separately allocated block of memory.

This member is mandatory and must be filled in.


### -field Privileges


<a href="https://msdn.microsoft.com/c9016511-740f-44f3-92ed-17cc518c6612">TOKEN_PRIVILEGES</a> structure that contains the <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">privileges</a> assigned to the user. This list of privileges will be augmented or overridden by any local security policy assigned privileges. 




Each privilege is expected to be in a separately allocated block of memory. The <a href="https://msdn.microsoft.com/c9016511-740f-44f3-92ed-17cc518c6612">TOKEN_PRIVILEGES</a> structure is also expected to be in a separately allocated block of memory.

If there are no privileges to assign to the user, this member may be set to <b>NULL</b>.


### -field Owner


<a href="https://msdn.microsoft.com/85617d56-ad46-40a3-a335-121f3c8edcc3">TOKEN_OWNER</a> structure. This member may be used to establish an explicit default owner. Normally, the user ID is used as the default owner. If another value is desired, it must be specified here. 




The <b>Owner.Sid</b> member may be set to <b>NULL</b> to indicate there is no alternate default owner value.


### -field DefaultDacl


<a href="https://msdn.microsoft.com/29fb738f-1ecd-4b72-9aea-64698cd74c12">TOKEN_DEFAULT_DACL</a> structure. This member may be used to establish a default protection for the user. If no value is provided, a default protection that grants everyone all access will be established. 




The <b>DefaultDacl.DefaultDacl</b> member may be set to <b>NULL</b> to indicate there is no default protection.


### -field UserClaims


<a href="https://msdn.microsoft.com/730541ED-0E33-4F19-BB99-145131161355">TOKEN_USER_CLAIMS</a> structure. This member stores the opaque user claims BLOB for the token. The <b>UserClaims</b> member may be set to <b>NULL</b> to indicate there are no additional user claims in the token. Claims are allow-only entities so omitting claims may restrict access.


### -field DeviceClaims


<a href="https://msdn.microsoft.com/FF20B64C-BD5F-45F5-83F1-B52634BE1065">TOKEN_DEVICE_CLAIMS</a> structure. This member stores the opaque device claims BLOB for the token. The <b>DeviceClaims</b> member may be set to <b>NULL</b> to indicate there are no additional device claims in the token. Claims are allow-only entities so omitting claims may restrict access.
					


### -field DeviceGroups


<a href="https://msdn.microsoft.com/387dd7f8-4177-40fa-b5fd-bb4b371a0e64">TOKEN_GROUPS</a> structure that contains the SIDs of the groups for the authenticating device member. As with user groups, this should not include WORLD or other system defined or assigned SIDs. The <b>DeviceGroups</b> member may be set to <b>NULL</b> to indicate that no compounding should occur. If <b>DeviceGroups</b> are present, LSA will add WORLD and other assigned SIDs. 

Unlike user groups, there is no notion of a primary device group.

Each SID is expected to be in a separately allocated block of memory. The <a href="https://msdn.microsoft.com/387dd7f8-4177-40fa-b5fd-bb4b371a0e64">TOKEN_GROUPS</a> structure is also expected to be in a separately allocated block of memory.

