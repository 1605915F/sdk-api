---
UID: NF:certenroll.IX509CertificateRequest.get_Silent
title: IX509CertificateRequest::get_Silent
author: windows-sdk-content
description: Specifies or retrieves a Boolean value that indicates whether any of the key-related modal dialogs are displayed during the certificate enrollment process.
old-location: security\ix509certificaterequest_silent_property.htm
tech.root: seccertenroll
ms.assetid: 339c8d47-4406-4f2e-b927-b2dd5f58d1ec
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IX509CertificateRequest interface [Security],Silent property, IX509CertificateRequest.Silent, IX509CertificateRequest.get_Silent, IX509CertificateRequest::Silent, IX509CertificateRequest::get_Silent, IX509CertificateRequest::put_Silent, Silent property [Security], Silent property [Security],IX509CertificateRequest interface, certenroll/IX509CertificateRequest::Silent, certenroll/IX509CertificateRequest::get_Silent, certenroll/IX509CertificateRequest::put_Silent, get_Silent, security.ix509certificaterequest_silent_property
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
 - IX509CertificateRequest.Silent
 - IX509CertificateRequest.get_Silent
 - IX509CertificateRequest.put_Silent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509CertificateRequest::get_Silent


## -description


The <b>Silent</b> property specifies or retrieves a Boolean value that indicates whether any of the  key-related modal dialogs are displayed during the certificate enrollment process.

This property is read/write.


## -parameters


## -remarks



This property value is used by key-related Certificate Enrollment Control modal dialogs that:<ul>
<li>Direct a user to insert a smart card</li>
<li>Request a smart card pin number</li>
<li>Request the  protection level for a new key</li>
<li>Request a user password before accessing a key</li>
</ul>


You can set this property before calling any initialization  method or the <a href="https://msdn.microsoft.com/098788f4-539f-420b-a4e1-65625dd56ca1">Encode</a> method. For a PKCS #10 request, the property value is retrieved from and specified on the associated <a href="https://msdn.microsoft.com/72612ea4-ed45-46ac-9dad-614a9a754d83">IX509PrivateKey</a> object if the key exists. For a PKCS #7 or CMC request the property value is updated on the inner request and all signing certificates.

If the certificate request contains nested requests and you set the <b>Silent</b> property on the top level request, it is automatically propagated to all of the inner requests. You can, however, set the property manually on each of the inner objects.




## -see-also




<a href="https://msdn.microsoft.com/5425c9ab-565d-449d-87e1-e5765868acfb">IX509CertificateRequest</a>



<a href="https://msdn.microsoft.com/7197a225-b2dc-47bb-8843-d3fb4bf95811">IX509CertificateRequestCertificate</a>



<a href="https://msdn.microsoft.com/77059388-c442-4db5-ab27-1db25e2f63b9">IX509CertificateRequestCmc</a>



<a href="https://msdn.microsoft.com/5b3764dc-fc63-45cc-8c35-65539c461e81">IX509CertificateRequestPkcs10</a>



<a href="https://msdn.microsoft.com/ae869557-6523-4387-835e-c9631898d864">IX509CertificateRequestPkcs7</a>



<a href="https://msdn.microsoft.com/25774ccb-8e76-443d-89da-177d6e77c019">IX509SignatureInformation</a>
 

 

