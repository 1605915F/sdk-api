---
UID: NS:bcrypt._CRYPT_PROVIDERS
title: CRYPT_PROVIDERS (bcrypt.h)
author: windows-sdk-content
description: Contains information about the registered CNG providers.
old-location: security\crypt_providers.htm
tech.root: SecCNG
ms.assetid: aef0e173-d3df-466e-ac2a-c686cae5edc9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PCRYPT_PROVIDERS, CRYPT_PROVIDERS, CRYPT_PROVIDERS structure [Security], PCRYPT_PROVIDERS, PCRYPT_PROVIDERS structure pointer [Security], bcrypt/CRYPT_PROVIDERS, bcrypt/PCRYPT_PROVIDERS, security.crypt_providers"
ms.topic: struct
req.header: bcrypt.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Bcrypt.h
api_name:
 - CRYPT_PROVIDERS
product: Windows
targetos: Windows
req.typenames: CRYPT_PROVIDERS, *PCRYPT_PROVIDERS
req.redist: 
---

# CRYPT_PROVIDERS structure


## -description


The <b>CRYPT_PROVIDERS</b> structure contains information about the registered CNG providers.


## -struct-fields




### -field cProviders

Contains the number of elements in the <b>rgpszProviders</b> array.


### -field rgpszProviders

An array of null-terminated Unicode strings that contains the names of the registered providers.


## -see-also




<a href="https://msdn.microsoft.com/a01adfec-dbe0-4817-af97-63163760fafc">BCryptEnumRegisteredProviders</a>
 

 

