---
UID: NF:certenroll.IX509CertificateRequestPkcs10.get_CriticalExtensions
title: IX509CertificateRequestPkcs10::get_CriticalExtensions (certenroll.h)
author: windows-sdk-content
description: Retrieves an IObjectIds collection that identifies the version 3 certificate extensions marked as critical.
old-location: security\ix509certificaterequestpkcs10_criticalextensions_property.htm
tech.root: seccertenroll
ms.assetid: 7ecde7cb-1a73-4fee-a949-c4bb36e61547
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CriticalExtensions property [Security], CriticalExtensions property [Security],IX509CertificateRequestPkcs10 interface, IX509CertificateRequestPkcs10 interface [Security],CriticalExtensions property, IX509CertificateRequestPkcs10.CriticalExtensions, IX509CertificateRequestPkcs10.get_CriticalExtensions, IX509CertificateRequestPkcs10::CriticalExtensions, IX509CertificateRequestPkcs10::get_CriticalExtensions, certenroll/IX509CertificateRequestPkcs10::CriticalExtensions, certenroll/IX509CertificateRequestPkcs10::get_CriticalExtensions, get_CriticalExtensions, security.ix509certificaterequestpkcs10_criticalextensions_property
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
 - IX509CertificateRequestPkcs10.CriticalExtensions
 - IX509CertificateRequestPkcs10.get_CriticalExtensions
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IX509CertificateRequestPkcs10::get_CriticalExtensions


## -description


The <b>CriticalExtensions</b> property retrieves an <a href="https://msdn.microsoft.com/f376a33e-005b-4810-9a26-b642236ff7af">IObjectIds</a> collection that identifies the version 3 certificate extensions marked as critical.

This property is read-only.


## -parameters


## -remarks



The extension criticality indicates to an application that uses certificates whether it can ignore the extension. You must initialize the <a href="https://msdn.microsoft.com/5b3764dc-fc63-45cc-8c35-65539c461e81">IX509CertificateRequestPkcs10</a> object before calling this property. For more information, see any of the following methods:

<ul>
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
 

 

