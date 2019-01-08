---
UID: NS:cryptxml._CRYPT_XML_KEYINFO_PARAM
title: CRYPT_XML_KEYINFO_PARAM
author: windows-sdk-content
description: Is used by the CryptXmlSign function to specify the members of the KeyInfo element to be encoded.
old-location: security\crypt_xml_keyinfo_param.htm
tech.root: SecCrypto
ms.assetid: cbde3f67-d948-452a-9958-52563dc7a8b5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CRYPT_XML_KEYINFO_PARAM, CRYPT_XML_KEYINFO_PARAM structure [Security], cryptxml/CRYPT_XML_KEYINFO_PARAM, security.crypt_xml_keyinfo_param
ms.topic: struct
req.header: cryptxml.h
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
 - Cryptxml.h
api_name:
 - CRYPT_XML_KEYINFO_PARAM
product: Windows
targetos: Windows
req.typenames: CRYPT_XML_KEYINFO_PARAM
req.redist: 
---

# CRYPT_XML_KEYINFO_PARAM structure


## -description


The <b>CRYPT_XML_KEYINFO_PARAM</b> structure is used by the <a href="https://msdn.microsoft.com/38bd365e-bc63-498c-a650-471429f09d37">CryptXmlSign</a> function to specify the members of the <b>KeyInfo</b> element to be encoded.


## -struct-fields




### -field wszId

A pointer to a null-terminated wide character string that contains the <b>Id</b> attribute of the <b>KeyInfo</b> element.


### -field wszKeyName

A pointer to a null-terminated wide character string that contains the value in the <b>KeyName</b> element.


### -field SKI

A <a href="https://msdn.microsoft.com/1c2a07b8-f702-47f3-8d4c-6ac0cbc63f0f">CERT_BLOB</a> structure that contains the value of the <b>X509SKI</b> element.


### -field wszSubjectName

A pointer to a null-terminated wide character string that  contains the value of the <b>X509SubjectName</b> element.


### -field cCertificate

The number of elements in the array pointed to by the <b>rgCertificate</b> member.


### -field rgCertificate

A pointer to an array of <a href="https://msdn.microsoft.com/1c2a07b8-f702-47f3-8d4c-6ac0cbc63f0f">CERT_BLOB</a> structures that are used to populate the <b>X509Certificate</b> elements.


### -field cCRL

The number of elements in the array pointed to by the <b>rgCRL</b> member.


### -field rgCRL

A pointer to an array of <a href="https://msdn.microsoft.com/1c2a07b8-f702-47f3-8d4c-6ac0cbc63f0f">CERT_BLOB</a> structures that are used to populate the <b>X509CRL</b> elements.

