---
UID: NE:ntsecpkg._SECPKG_SESSIONINFO_TYPE
title: SECPKG_SESSIONINFO_TYPE (ntsecpkg.h)
author: windows-sdk-content
description: Specifies the format of session information.
old-location: security\secpkg_sessioninfo_type.htm
tech.root: SecAuthN
ms.assetid: 462b028a-9f74-4367-b89b-97fd9be301ed
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: SECPKG_SESSIONINFO_TYPE, SECPKG_SESSIONINFO_TYPE enumeration [Security], SecSessionPrimaryCred, ntsecpkg/SECPKG_SESSIONINFO_TYPE, ntsecpkg/SecSessionPrimaryCred, security.secpkg_sessioninfo_type
ms.topic: enum
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
 - HeaderDef
api_location:
 - Ntsecpkg.h
api_name:
 - SECPKG_SESSIONINFO_TYPE
product: Windows
targetos: Windows
req.typenames: SECPKG_SESSIONINFO_TYPE
req.redist: 
ms.custom: 19H1
---

# SECPKG_SESSIONINFO_TYPE enumeration


## -description


Specifies the format of session information. This enumeration is used by the <a href="https://msdn.microsoft.com/1f12d8a4-6cbd-43e3-98a7-eaf3d30a053e">CreateTokenEx</a> function to specify the format of the <i>SessionInformation</i> parameter.


## -enum-fields




### -field SecSessionPrimaryCred

The session information is contained in a <a href="https://msdn.microsoft.com/e51fd400-6c3c-4861-ab5c-6c1800b12d31">SECPKG_PRIMARY_CRED</a> structure.

