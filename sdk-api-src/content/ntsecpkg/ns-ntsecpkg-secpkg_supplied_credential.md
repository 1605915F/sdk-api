---
UID: NS:ntsecpkg._SECPKG_SUPPLIED_CREDENTIAL
title: SECPKG_SUPPLIED_CREDENTIAL (ntsecpkg.h)
author: windows-sdk-content
description: Specifies the supplied credentials.
old-location: security\secpkg_supplied_credential.htm
tech.root: SecAuthN
ms.assetid: 23849312-7AC5-4D09-8889-27DFF8E32FE8
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PSECPKG_SUPPLIED_CREDENTIAL, PSECPKG_SUPPLIED_CREDENTIAL, PSECPKG_SUPPLIED_CREDENTIAL structure pointer [Security], SECPKG_SUPPLIED_CREDENTIAL, SECPKG_SUPPLIED_CREDENTIAL structure [Security], ntsecpkg/PSECPKG_SUPPLIED_CREDENTIAL, ntsecpkg/SECPKG_SUPPLIED_CREDENTIAL, security.secpkg_supplied_credential"
ms.topic: struct
req.header: ntsecpkg.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - SECPKG_SUPPLIED_CREDENTIAL
product: Windows
targetos: Windows
req.typenames: SECPKG_SUPPLIED_CREDENTIAL, *PSECPKG_SUPPLIED_CREDENTIAL
req.redist: 
---

# SECPKG_SUPPLIED_CREDENTIAL structure


## -description


Specifies the supplied credentials.


## -struct-fields




### -field cbHeaderLength

The length of the header.


### -field cbStructureLength

Pay load length, including the header.


### -field UserName

The user name for Unicode only.


### -field DomainName

The domain name for Unicode only.


### -field PackedCredentials

The credentials in the <a href="https://msdn.microsoft.com/9a21f0cd-d4e1-4aa8-8d0d-72bc7002ce32">SEC_WINNT_AUTH_PACKED_CREDENTIALS</a> structure.


### -field CredFlags

The authentication identity flags.

