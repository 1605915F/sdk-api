---
UID: NF:certenroll.ICertificatePolicy.get_PolicyQualifiers
title: ICertificatePolicy::get_PolicyQualifiers (certenroll.h)
author: windows-sdk-content
description: Retrieves a collection of optional policy qualifiers that can be applied to a certificate policy.
old-location: security\icertificatepolicy_policyqualifiers_property.htm
tech.root: seccertenroll
ms.assetid: 7955dfa1-70b2-4b6e-975f-c489a6284c5c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ICertificatePolicy interface [Security],PolicyQualifiers property, ICertificatePolicy.PolicyQualifiers, ICertificatePolicy.get_PolicyQualifiers, ICertificatePolicy::PolicyQualifiers, ICertificatePolicy::get_PolicyQualifiers, PolicyQualifiers property [Security], PolicyQualifiers property [Security],ICertificatePolicy interface, certenroll/ICertificatePolicy::PolicyQualifiers, certenroll/ICertificatePolicy::get_PolicyQualifiers, get_PolicyQualifiers, security.icertificatepolicy_policyqualifiers_property
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
 - ICertificatePolicy.PolicyQualifiers
 - ICertificatePolicy.get_PolicyQualifiers
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ICertificatePolicy::get_PolicyQualifiers


## -description


The <b>PolicyQualifiers</b> property retrieves a collection of optional policy qualifiers that can be applied to a certificate policy.

This property is read-only.


## -parameters


## -remarks



An empty <a href="https://msdn.microsoft.com/da8b6289-379e-4dff-b15a-b0967f245c3d">IPolicyQualifiers</a> object is created when you call the <a href="https://msdn.microsoft.com/995b344b-ed1f-47e4-a7c6-0d638ed9ec23">Initialize</a> method. You can call the <b>PolicyQualifiers</b> property to retrieve this object and specify qualifying information for the policy. Policy qualifiers only apply if you are creating a <b>CertificatePolicies</b> extension. For more information, see the <a href="https://msdn.microsoft.com/d35d155c-fb81-4d7e-b5c9-82ac5af4b79e">IX509ExtensionCertificatePolicies</a>.




## -see-also




<a href="https://msdn.microsoft.com/2503adcb-0b73-42ef-98cf-a2b906e34ef7">ICertificatePolicies</a>



<a href="https://msdn.microsoft.com/2162de70-edcc-4f01-807d-79ff200d0016">ICertificatePolicy</a>
 

 

