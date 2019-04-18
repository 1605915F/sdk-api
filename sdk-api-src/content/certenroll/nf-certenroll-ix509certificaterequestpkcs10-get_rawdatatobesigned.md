---
UID: NF:certenroll.IX509CertificateRequestPkcs10.get_RawDataToBeSigned
title: IX509CertificateRequestPkcs10::get_RawDataToBeSigned (certenroll.h)
author: windows-sdk-content
description: Retrieves the unsigned certificate request created by the Encode method.
old-location: security\ix509certificaterequestpkcs10_rawdatatobesigned_property.htm
tech.root: seccertenroll
ms.assetid: 43e7e3e2-d94d-46b4-b76b-cd54f9d618ec
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IX509CertificateRequestPkcs10 interface [Security],RawDataToBeSigned property, IX509CertificateRequestPkcs10.RawDataToBeSigned, IX509CertificateRequestPkcs10.get_RawDataToBeSigned, IX509CertificateRequestPkcs10::RawDataToBeSigned, IX509CertificateRequestPkcs10::get_RawDataToBeSigned, RawDataToBeSigned property [Security], RawDataToBeSigned property [Security],IX509CertificateRequestPkcs10 interface, certenroll/IX509CertificateRequestPkcs10::RawDataToBeSigned, certenroll/IX509CertificateRequestPkcs10::get_RawDataToBeSigned, get_RawDataToBeSigned, security.ix509certificaterequestpkcs10_rawdatatobesigned_property
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
 - IX509CertificateRequestPkcs10.RawDataToBeSigned
 - IX509CertificateRequestPkcs10.get_RawDataToBeSigned
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IX509CertificateRequestPkcs10::get_RawDataToBeSigned


## -description


The <b>RawDataToBeSigned</b> property retrieves  the unsigned certificate request created by the <a href="https://msdn.microsoft.com/098788f4-539f-420b-a4e1-65625dd56ca1">Encode</a> method.   The request is contained in a byte array encoded by using <a href="https://msdn.microsoft.com/d007cbb9-b547-4dc7-bc22-b526f650f7c2">Distinguished Encoding Rules</a> (DER) as defined by the <a href="https://msdn.microsoft.com/0baaa937-f635-4500-8dcd-9dbbd6f4cd02">Abstract Syntax Notation One</a> (ASN.1) standard. The DER-encoded byte array is represented by a string that is either a pure binary sequence or is Unicode encoded.

This property is read-only.


## -parameters


## -remarks



The <a href="https://msdn.microsoft.com/098788f4-539f-420b-a4e1-65625dd56ca1">Encode</a> method creates a DER-encoded and signed certificate request, but it also internally saves the unsigned request as a byte array. You can use the <b>RawDataToBeSigned</b> property to retrieve that binary data as an Unicode-encoded string.

 You must initialize the <a href="https://msdn.microsoft.com/5b3764dc-fc63-45cc-8c35-65539c461e81">IX509CertificateRequestPkcs10</a> object and call  <a href="https://msdn.microsoft.com/098788f4-539f-420b-a4e1-65625dd56ca1">Encode</a> before calling this property. For more information, see any of the following methods:<ul>
<li>
<a href="https://msdn.microsoft.com/10ab62c3-9c6f-4e1b-8a86-131d08282d9c">InitializeDecode</a>
</li>
<li>
<a href="https://msdn.microsoft.com/3f390abc-5c1c-4f9c-a5f4-4d6fec065acf">InitializeFromCertificate</a>
</li>
<li>
<a href="https://msdn.microsoft.com/b26e69c4-bfe4-4395-aaf6-bc1d045f59cc">InitializeFromPrivateKey</a>
</li>
<li>
<a href="https://msdn.microsoft.com/7b7e00dc-649b-4bcb-a9b6-5745b33ea48b">InitializeFromPublicKey</a>
</li>
<li>
<a href="https://msdn.microsoft.com/4ea746c3-b967-41b4-94ae-7b16b93ca4e4">InitializeFromTemplateName</a>
</li>
</ul>





## -see-also




<a href="https://msdn.microsoft.com/5b3764dc-fc63-45cc-8c35-65539c461e81">IX509CertificateRequestPkcs10</a>
 

 

