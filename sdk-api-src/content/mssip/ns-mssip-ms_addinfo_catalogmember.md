---
UID: NS:mssip.MS_ADDINFO_CATALOGMEMBER_
title: MS_ADDINFO_CATALOGMEMBER
author: windows-sdk-content
description: Provides additional information for catalog member subject types.
old-location: security\ms_addinfo_catalogmember.htm
tech.root: SecCrypto
ms.assetid: 40a00c8a-95e4-406c-b04e-0d29beb70d67
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMS_ADDINFO_CATALOGMEMBER, MS_ADDINFO_CATALOGMEMBER, MS_ADDINFO_CATALOGMEMBER structure [Security], PMS_ADDINFO_CATALOGMEMBER, PMS_ADDINFO_CATALOGMEMBER structure pointer [Security], mssip/MS_ADDINFO_CATALOGMEMBER_, mssip/PMS_ADDINFO_CATALOGMEMBER, security.ms_addinfo_catalogmember"
ms.topic: struct
req.header: mssip.h
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
 - Mssip.h
api_name:
 - MS_ADDINFO_CATALOGMEMBER
product: Windows
targetos: Windows
req.typenames: MS_ADDINFO_CATALOGMEMBER, *PMS_ADDINFO_CATALOGMEMBER
req.redist: 
---

# MS_ADDINFO_CATALOGMEMBER structure


## -description


The <b>MS_ADDINFO_CATALOGMEMBER</b> structure provides additional information for catalog member subject types.


## -struct-fields




### -field cbStruct

The size, in bytes, of this structure.


### -field pStore

A <a href="https://msdn.microsoft.com/65a15797-453c-4f47-8ea1-c92e616b50aa">CRYPTCATSTORE</a> structure that contains a catalog file store.


### -field pMember

A <a href="https://msdn.microsoft.com/08f663d9-9dc2-4ac9-95c5-7f2ed972eb9b">CRYPTCATMEMBER</a> structure that contains a catalog member.

