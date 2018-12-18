---
UID: NC:wincrypt.PFN_CRYPT_ENUM_OID_INFO
title: PFN_CRYPT_ENUM_OID_INFO
author: windows-sdk-content
description: The CRYPT_ENUM_OID_INFO callback function is used with the CryptEnumOIDInfo function.
old-location: security\crypt_enum_oid_info.htm
tech.root: seccrypto
ms.assetid: 30ae4274-631d-4c6a-96c5-18f096607cad
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CRYPT_ENUM_OID_INFO, CRYPT_ENUM_OID_INFO callback function [Security], PFN_CRYPT_ENUM_OID_INFO, PFN_CRYPT_ENUM_OID_INFO callback, security.crypt_enum_oid_info, wincrypt/CRYPT_ENUM_OID_INFO
ms.topic: callback
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
 - UserDefined
api_location:
 - Wincrypt.h
api_name:
 - CRYPT_ENUM_OID_INFO
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PFN_CRYPT_ENUM_OID_INFO callback function


## -description


The <b>CRYPT_ENUM_OID_INFO</b> callback function  is used with the <a href="https://msdn.microsoft.com/6af23bb4-3a27-425a-90bb-9a69ea081b25">CryptEnumOIDInfo</a> function.


## -parameters




### -param pInfo [in]

A pointer to the OID information.


### -param *pvArg [in]

A pointer to arguments passed through to the callback function.


## -returns



Returns <b>TRUE</b> to continue the enumeration and <b>FALSE</b> to stop the enumeration.
 If <b>FALSE</b> is returned, the <a href="https://msdn.microsoft.com/6af23bb4-3a27-425a-90bb-9a69ea081b25">CryptEnumOIDInfo</a> enumeration is stopped.




## -see-also




<a href="https://msdn.microsoft.com/6af23bb4-3a27-425a-90bb-9a69ea081b25">CryptEnumOIDInfo</a>
 

 

