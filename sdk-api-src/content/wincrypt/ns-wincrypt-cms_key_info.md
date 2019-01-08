---
UID: NS:wincrypt._CMS_KEY_INFO
title: CMS_KEY_INFO
author: windows-sdk-content
description: Not used.
old-location: security\cms_key_info.htm
tech.root: SecCrypto
ms.assetid: 4aec1184-d375-48a0-8b98-d5ff5932d297
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCMS_KEY_INFO, CMS_KEY_INFO, CMS_KEY_INFO structure [Security], PCMS_KEY_INFO, PCMS_KEY_INFO structure pointer [Security], security.cms_key_info, wincrypt/CMS_KEY_INFO, wincrypt/PCMS_KEY_INFO"
ms.topic: struct
req.header: wincrypt.h
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
 - Wincrypt.h
api_name:
 - CMS_KEY_INFO
product: Windows
targetos: Windows
req.typenames: CMS_KEY_INFO, *PCMS_KEY_INFO
req.redist: 
---

# CMS_KEY_INFO structure


## -description


The <b>CMS_KEY_INFO</b> structure is not used.


## -struct-fields




### -field dwVersion

The size, in bytes, of this structure.


### -field Algid

One of the <a href="https://msdn.microsoft.com/557436b4-f7f1-4708-acc7-c6b47e6322ad">ALG_ID</a> values that identifies the algorithm for the key to be converted.


### -field pbOID

The address of a buffer that contains additional public information. This member is optional and can be <b>NULL</b> if this is not needed.


### -field cbOID

The size, in bytes, of the <b>pbOID</b> buffer. This member should be zero if <b>pbOID</b> is not used.

