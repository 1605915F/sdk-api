---
UID: NF:certenroll.IX509AttributeArchiveKey.get_EncryptedKeyBlob
title: IX509AttributeArchiveKey::get_EncryptedKeyBlob
author: windows-sdk-content
description: Retrieves a byte array that contains the encrypted key.
old-location: security\ix509attributearchivekey_encryptedkeyblob_property.htm
tech.root: seccertenroll
ms.assetid: 3230cfbf-5486-4f77-9efe-5bc542e3e096
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EncryptedKeyBlob property [Security], EncryptedKeyBlob property [Security],IX509AttributeArchiveKey interface, IX509AttributeArchiveKey interface [Security],EncryptedKeyBlob property, IX509AttributeArchiveKey.EncryptedKeyBlob, IX509AttributeArchiveKey.get_EncryptedKeyBlob, IX509AttributeArchiveKey::EncryptedKeyBlob, IX509AttributeArchiveKey::get_EncryptedKeyBlob, certenroll/IX509AttributeArchiveKey::EncryptedKeyBlob, certenroll/IX509AttributeArchiveKey::get_EncryptedKeyBlob, get_EncryptedKeyBlob, security.ix509attributearchivekey_encryptedkeyblob_property
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
 - IX509AttributeArchiveKey.EncryptedKeyBlob
 - IX509AttributeArchiveKey.get_EncryptedKeyBlob
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509AttributeArchiveKey::get_EncryptedKeyBlob


## -description


The <b>EncryptedKeyBlob</b> property retrieves a byte array that contains the encrypted key. The byte array is represented by a Unicode-encoded string.

This property is read-only.


## -parameters


## -remarks



Call the <a href="https://msdn.microsoft.com/en-us/library/Aa377070(v=VS.85).aspx">InitializeEncode</a> method or the  <a href="https://msdn.microsoft.com/en-us/library/Aa377069(v=VS.85).aspx">InitializeDecode</a> method to initialize the <b>EncryptedKeyBlob</b> property. You can call the following properties to retrieve the raw data:

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa377067(v=VS.85).aspx">EncryptionAlgorithm</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/Aa377068(v=VS.85).aspx">EncryptionStrength</a>
</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa377059(v=VS.85).aspx">IX509AttributeArchiveKey</a>
 

 

