---
UID: NF:certenroll.IX509AttributeArchiveKey.get_EncryptionStrength
title: IX509AttributeArchiveKey::get_EncryptionStrength
author: windows-sdk-content
description: Retrieves an integer that contains the encryption strength of the symmetric algorithm used to encrypt the key.
old-location: security\ix509attributearchivekey_encryptionstrength_property.htm
tech.root: seccertenroll
ms.assetid: c365a2e0-caff-4c92-aa22-33c165ea672e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EncryptionStrength property [Security], EncryptionStrength property [Security],IX509AttributeArchiveKey interface, IX509AttributeArchiveKey interface [Security],EncryptionStrength property, IX509AttributeArchiveKey.EncryptionStrength, IX509AttributeArchiveKey.get_EncryptionStrength, IX509AttributeArchiveKey::EncryptionStrength, IX509AttributeArchiveKey::get_EncryptionStrength, certenroll/IX509AttributeArchiveKey::EncryptionStrength, certenroll/IX509AttributeArchiveKey::get_EncryptionStrength, get_EncryptionStrength, security.ix509attributearchivekey_encryptionstrength_property
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenroll.h
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
req.dll: CertEnroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CertEnroll.dll
api_name:
 - IX509AttributeArchiveKey.EncryptionStrength
 - IX509AttributeArchiveKey.get_EncryptionStrength
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509AttributeArchiveKey::get_EncryptionStrength


## -description


The <b>EncryptionStrength</b> property retrieves an integer that contains the encryption strength of the symmetric algorithm used to encrypt the key.

This property is read-only.


## -parameters


## -remarks



You can specify this property by calling the <a href="https://msdn.microsoft.com/en-us/library/Aa377070(v=VS.85).aspx">InitializeEncode</a> method or the  <a href="https://msdn.microsoft.com/en-us/library/Aa377069(v=VS.85).aspx">InitializeDecode</a> method. However, the property is currently ignored and zero is returned because the Certificate Enrollment SDK does not support any algorithms for which the <a href="https://msdn.microsoft.com/en-us/library/ms721599(v=VS.85).aspx">object identifier</a> (OID) does not already imply the encryption strength (key length). For example, AES has multiple strengths, but each strength is already indicated by the OID. 

You can call the following properties to retrieve the raw data:<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa377067(v=VS.85).aspx">EncryptionAlgorithm</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa377066(v=VS.85).aspx">EncryptedKeyBlob</a>
</li>
</ul>





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa377059(v=VS.85).aspx">IX509AttributeArchiveKey</a>
 

 

