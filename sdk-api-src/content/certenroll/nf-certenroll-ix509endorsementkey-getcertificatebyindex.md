---
UID: NF:certenroll.IX509EndorsementKey.GetCertificateByIndex
title: IX509EndorsementKey::GetCertificateByIndex
author: windows-sdk-content
description: Gets the endorsement certificate associated with the endorsement key from the key storage provider for the specified index.
old-location: security\ix509endorsementkey_getcertificatebyindex.htm
tech.root: seccertenroll
ms.assetid: ab1eb37a-d79e-4d02-8e60-6c093f42c68f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCertificateByIndex, GetCertificateByIndex method [Security], GetCertificateByIndex method [Security],IX509EndorsementKey interface, IX509EndorsementKey interface [Security],GetCertificateByIndex method, IX509EndorsementKey.GetCertificateByIndex, IX509EndorsementKey::GetCertificateByIndex, certenroll/IX509EndorsementKey::GetCertificateByIndex, security.ix509endorsementkey_getcertificatebyindex
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certenroll.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Certenroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certenroll.dll
api_name:
 - IX509EndorsementKey.GetCertificateByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509EndorsementKey::GetCertificateByIndex


## -description


Gets the endorsement certificate associated with the endorsement key from the key storage provider for the specified index. You can only call the <b>GetCertificateByIndex</b> method after the <a href="https://msdn.microsoft.com/en-us/library/Dn379364(v=VS.85).aspx">Open</a> method has been successfully called.


## -parameters




### -param ManufacturerOnly [in]

True to get manufacturer endorsement keys only; otherwise false. The default is false.


### -param dwIndex [in]

The index of the requested endorsement certificate.


### -param Encoding [in]

An <a href="https://msdn.microsoft.com/en-us/library/Aa374936(v=VS.85).aspx">EncodingType</a> enumeration value that specifies the type of Unicode-encoding applied to the  endorsement certificate. The default value is XCN_CRYPT_STRING_BASE64.


### -param pValue [out, retval]

The endorsement certificate requested.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn379356(v=VS.85).aspx">IX509EndorsementKey</a>
 

 

