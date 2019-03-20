---
UID: NN:certenroll.ICertPropertyEnrollment
title: ICertPropertyEnrollment (certenroll.h)
author: windows-sdk-content
description: Represents a certificate property that contains certificate and certification authority (CA) information created when the client calls the Enroll method on the IX509Enrollment interface.
old-location: security\icertpropertyenrollment.htm
tech.root: seccertenroll
ms.assetid: 7530998b-b59c-426b-a74a-ead4bca55c3b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICertPropertyEnrollment, ICertPropertyEnrollment interface [Security], ICertPropertyEnrollment interface [Security],described, certenroll/ICertPropertyEnrollment, security.icertpropertyenrollment
ms.topic: interface
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
 - ICertPropertyEnrollment
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertPropertyEnrollment interface


## -description


The <b>ICertPropertyEnrollment</b> interface represents a certificate property that contains certificate and certification authority (CA) information created when the client calls the <a href="https://msdn.microsoft.com/63abecac-39f4-497a-8851-7a2260abc3dd">Enroll</a> method on the <a href="https://msdn.microsoft.com/37f1dd3b-bbe9-40ab-87c9-2405d97f5541">IX509Enrollment</a> interface. The property value consists of the following information:<ul>
<li>A certificate request ID</li>
<li>The common name (CN) of the certificate subject</li>
<li>The certification authority (CA) Domain Name System (DNS) name</li>
<li>The optional display name of the certificate being requested</li>
</ul>


This property is initialized by the enrollment process and associated with the dummy certificate that is temporarily copied to the request store. If the CA marks the request pending after it is submitted, auto-enrollment can later use the request ID to retrieve the certificate response. If the CA denies the certificate request, the dummy certificate in the request store and all properties associated with it are deleted. If the CA issues the certificate and it is installed in the personal store, this property is associated with the new certificate and the dummy certificate is deleted.<div class="alert"><b>Note</b>  The <a href="https://msdn.microsoft.com/e7ad0ec5-a568-4506-ba54-908e00083c2b">CERTENROLL_PROPERTYID</a> value is XCN_CERT_ENROLLMENT_PROP_ID.</div>
<div> </div>



## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ICertPropertyEnrollment</b> interface inherits from <a href="https://msdn.microsoft.com/947c2f09-993d-4ced-8b76-66b79d96e3bc">ICertProperty</a>. <b>ICertPropertyEnrollment</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
<li><a href="https://docs.microsoft.com/">Properties</a></li>
</ul>

## -members

The <b>ICertPropertyEnrollment</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/47e9b11f-3f23-4e2f-817a-4b6311e3d710">Initialize</a>
</td>
<td align="left" width="63%">
Initializes the property from the certificate request ID, the certification authority configuration string, and a certificate display name.

</td>
</tr>
</table> 
<h3><a id="properties"></a>Properties</h3>The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ICertPropertyEnrollment</b> interface has these properties.
<table class="members" id="memberListProperties">
<tr>
<th align="left" width="27%">Property</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/5b388cfe-e0b1-4b57-bf6c-81f9ab65ffcf">CADnsName</a>


</td>
<td align="left" width="63%">
Retrieves the DNS name of the certification authority.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/ea490e37-e1b9-4887-8051-c3447136875c">CAName</a>


</td>
<td align="left" width="63%">
Retrieves the common name of the certification authority.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/a12b7368-cace-47c4-bfd4-08845dc2634c">FriendlyName</a>


</td>
<td align="left" width="63%">
Retrieves the display name of the certificate.

</td>
</tr>
<tr data="declared;">
<td align="left" width="27%" xml:space="preserve">

<a href="https://msdn.microsoft.com/a9e2000c-7d64-43f1-b891-b5cd6f46201f">RequestId</a>


</td>
<td align="left" width="63%">
Retrieves a unique  certificate request identifier.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/d49511ed-8651-457e-a102-0bea4edde24c">CertEnroll Interfaces</a>



<a href="https://msdn.microsoft.com/947c2f09-993d-4ced-8b76-66b79d96e3bc">ICertProperty</a>
 

 

