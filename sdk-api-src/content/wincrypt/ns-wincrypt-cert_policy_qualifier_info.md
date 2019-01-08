---
UID: NS:wincrypt._CERT_POLICY_QUALIFIER_INFO
title: CERT_POLICY_QUALIFIER_INFO
author: windows-sdk-content
description: The CERT_POLICY_QUALIFIER_INFO structure contains an object identifier (OID) specifying the qualifier and qualifier-specific supplemental information.
old-location: security\cert_policy_qualifier_info.htm
tech.root: SecCrypto
ms.assetid: 86b1716d-541f-4e06-a824-01c22f0eba27
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCERT_POLICY_QUALIFIER_INFO, CERT_POLICY_QUALIFIER_INFO, CERT_POLICY_QUALIFIER_INFO structure [Security], PCERT_POLICY_QUALIFIER_INFO, PCERT_POLICY_QUALIFIER_INFO structure pointer [Security], _crypto2_cert_policy_qualifier_info, security.cert_policy_qualifier_info, wincrypt/CERT_POLICY_QUALIFIER_INFO, wincrypt/PCERT_POLICY_QUALIFIER_INFO"
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
 - CERT_POLICY_QUALIFIER_INFO
product: Windows
targetos: Windows
req.typenames: CERT_POLICY_QUALIFIER_INFO, *PCERT_POLICY_QUALIFIER_INFO
req.redist: 
---

# CERT_POLICY_QUALIFIER_INFO structure


## -description


The <b>CERT_POLICY_QUALIFIER_INFO</b> structure contains an object identifier (OID) specifying the qualifier and qualifier-specific supplemental information.

The <b>CERT_POLICY_QUALIFIER_INFO</b> structure is a component of 
<a href="https://msdn.microsoft.com/0d6396fe-99f6-4f66-9f01-55582d24ddc1">CERT_POLICY_INFO</a>.


## -struct-fields




### -field pszPolicyQualifierId

OID specifying the qualifier.
					


### -field Qualifier

A <a href="https://msdn.microsoft.com/7a06eae5-96d8-4ece-98cb-cf0710d2ddbd">CRYPT_OBJID_BLOB</a> structure that contains qualifier specific supplemental information.


## -see-also




<a href="https://msdn.microsoft.com/0d6396fe-99f6-4f66-9f01-55582d24ddc1">CERT_POLICY_INFO</a>



<a href="https://msdn.microsoft.com/7a06eae5-96d8-4ece-98cb-cf0710d2ddbd">CRYPT_INTEGER_BLOB</a>
 

 

