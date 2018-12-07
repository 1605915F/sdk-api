---
UID: NS:cryptxml._CRYPT_XML_KEY_RSA_KEY_VALUE
title: "_CRYPT_XML_KEY_RSA_KEY_VALUE"
author: windows-sdk-content
description: Defines an RSA key value. The CRYPT_XML_KEY_RSA_KEY_VALUE structure is used as element of the key value union in the CRYPT_XML_KEY_VALUE structure.
old-location: security\crypt_xml_key_rsa_key_value.htm
tech.root: seccrypto
ms.assetid: e2b1344d-c108-4255-bd50-06d742ed67a8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CRYPT_XML_KEY_RSA_KEY_VALUE, CRYPT_XML_KEY_RSA_KEY_VALUE structure [Security], _CRYPT_XML_KEY_RSA_KEY_VALUE, cryptxml/CRYPT_XML_KEY_RSA_KEY_VALUE, security.crypt_xml_key_rsa_key_value
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - CRYPT_XML_KEY_RSA_KEY_VALUE
product: Windows
targetos: Windows
req.typenames: CRYPT_XML_KEY_RSA_KEY_VALUE
req.redist: 
---

# _CRYPT_XML_KEY_RSA_KEY_VALUE structure


## -description


The <b>CRYPT_XML_KEY_RSA_KEY_VALUE</b> structure defines an RSA key value.  The <b>CRYPT_XML_KEY_RSA_KEY_VALUE</b> structure is used as element of the key value union  in the <a href="https://msdn.microsoft.com/en-us/library/Dd433858(v=VS.85).aspx">CRYPT_XML_KEY_VALUE</a> structure.


## -struct-fields




### -field Modulus

A <a href="https://msdn.microsoft.com/en-us/library/Dd433847(v=VS.85).aspx">CRYPT_XML_DATA_BLOB</a> structure that contains the <a href="https://msdn.microsoft.com/en-us/library/ms721603(v=VS.85).aspx">public key</a> modulus data.


### -field Exponent

A <a href="https://msdn.microsoft.com/en-us/library/Dd433847(v=VS.85).aspx">CRYPT_XML_DATA_BLOB</a> structure that contains the public key exponent data.

