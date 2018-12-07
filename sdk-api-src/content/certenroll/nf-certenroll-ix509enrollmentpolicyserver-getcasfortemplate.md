---
UID: NF:certenroll.IX509EnrollmentPolicyServer.GetCAsForTemplate
title: IX509EnrollmentPolicyServer::GetCAsForTemplate
author: windows-sdk-content
description: Retrieves a collection of certificate enrollment servers that support a specified template.
old-location: security\ix509enrollmentpolicyserver_getcasfortemplate.htm
tech.root: seccertenroll
ms.assetid: 7330aea0-36b3-49fa-8970-2476f2ae9d34
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCAsForTemplate, GetCAsForTemplate method [Security], GetCAsForTemplate method [Security],IX509EnrollmentPolicyServer interface, IX509EnrollmentPolicyServer interface [Security],GetCAsForTemplate method, IX509EnrollmentPolicyServer.GetCAsForTemplate, IX509EnrollmentPolicyServer::GetCAsForTemplate, certenroll/IX509EnrollmentPolicyServer::GetCAsForTemplate, security.ix509enrollmentpolicyserver_getcasfortemplate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certenroll.h
api_name:
 - IX509EnrollmentPolicyServer.GetCAsForTemplate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509EnrollmentPolicyServer::GetCAsForTemplate


## -description


The <b>GetCAsForTemplate</b> method retrieves a collection of certificate enrollment servers that support a specified template.


## -parameters




### -param pTemplate [in]

Pointer to an <a href="https://msdn.microsoft.com/en-us/library/Ee351664(v=VS.85).aspx">IX509CertificateTemplate</a> interface that represents the template.


### -param ppCAs [out, retval]

Address of a variable that receives a pointer to an <a href="https://msdn.microsoft.com/en-us/library/Ee338611(v=VS.85).aspx">ICertificationAuthorities</a> interface that represents the server collection.


## -returns



If the function succeeds, the function returns <b>S_OK</b>.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following table.  For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>OLE_E_BLANK</b></dt>
</dl>
</td>
<td width="60%">
The <a href="https://msdn.microsoft.com/en-us/library/Ee351692(v=VS.85).aspx">IX509EnrollmentPolicyServer</a> object has not been initialized.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ee351692(v=VS.85).aspx">IX509EnrollmentPolicyServer</a>
 

 

