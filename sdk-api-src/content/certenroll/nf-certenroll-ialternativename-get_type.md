---
UID: NF:certenroll.IAlternativeName.get_Type
title: IAlternativeName::get_Type
author: windows-sdk-content
description: Retrieves the alternative name type.
old-location: security\ialternativename_type_property.htm
tech.root: seccertenroll
ms.assetid: fdb1a7db-20f6-4732-bb59-fc078387375d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAlternativeName interface [Security],Type property, IAlternativeName.Type, IAlternativeName.get_Type, IAlternativeName::Type, IAlternativeName::get_Type, Type property [Security], Type property [Security],IAlternativeName interface, certenroll/IAlternativeName::Type, certenroll/IAlternativeName::get_Type, get_Type, security.ialternativename_type_property
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
 - IAlternativeName.Type
 - IAlternativeName.get_Type
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAlternativeName::get_Type


## -description


The <b>Type</b> property retrieves the alternative name type.

This property is read-only.


## -parameters


## -remarks



The following values from the <a href="https://msdn.microsoft.com/79b675cc-c979-46ab-aee1-0031af2efd40">AlternativeNameType</a> enumeration can be returned. The  <b>XCN_CERT_ALT_NAME_UNKNOWN</b> value is never returned.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_OTHER_NAME</b></td>
<td>The name consists of an <a href="https://msdn.microsoft.com/e6be8932-015e-4058-b249-1671b3fea521">object identifier</a> (OID) and a byte array.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_RFC822_NAME</b></td>
<td>The name is an email address.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_DNS_NAME</b></td>
<td>The name is a DNS name.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_DIRECTORY_NAME</b></td>
<td>The name is an <a href="https://msdn.microsoft.com/28dba6ef-939f-4789-9789-ee6e0fef0177">X.500</a> directory name.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_URL</b></td>
<td>The name is a URL.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_IP_ADDRESS</b></td>
<td>The name is an IP address.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_REGISTERED_ID</b></td>
<td>The name is a registered OID.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_GUID</b></td>
<td>The name is a GUID.</td>
</tr>
<tr>
<td><b>XCN_CERT_ALT_NAME_USER_PRINCIPLE_NAME</b></td>
<td>The name is a <a href="https://msdn.microsoft.com/264f6cb6-36c6-4cdb-b7bb-a5dbd332adcb">user principal name</a> (UPN).</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/2a6cfda8-b3cb-4a0f-bb65-b182c16207be">IAlternativeName</a>
 

 

