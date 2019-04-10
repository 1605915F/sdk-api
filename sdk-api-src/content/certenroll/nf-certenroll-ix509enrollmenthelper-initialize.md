---
UID: NF:certenroll.IX509EnrollmentHelper.Initialize
title: IX509EnrollmentHelper::Initialize (certenroll.h)
author: windows-sdk-content
description: Initializes an IX509EnrollmentHelper object.
old-location: security\ix509enrollmenthelper_initialize.htm
tech.root: seccertenroll
ms.assetid: 83cb603b-9396-4983-8707-12d1c5b8b234
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ContextAdministratorForceMachine, ContextMachine, ContextUser, IX509EnrollmentHelper interface [Security],Initialize method, IX509EnrollmentHelper.Initialize, IX509EnrollmentHelper::Initialize, Initialize, Initialize method [Security], Initialize method [Security],IX509EnrollmentHelper interface, certenroll/IX509EnrollmentHelper::Initialize, security.ix509enrollmenthelper_initialize
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
 - IX509EnrollmentHelper.Initialize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509EnrollmentHelper::Initialize


## -description


The <b>Initialize</b> method initializes an <a href="https://msdn.microsoft.com/19124591-be1a-401e-9b83-c640d00de34a">IX509EnrollmentHelper</a> object.


## -parameters




### -param Context [in]

An <a href="https://msdn.microsoft.com/2db0e129-a566-47ba-ab57-53c7db09e8e3">X509CertificateEnrollmentContext</a> enumeration value that specifies the nature of the end entity for which the issued certificate is intended. This can be one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="ContextUser"></a><a id="contextuser"></a><a id="CONTEXTUSER"></a><dl>
<dt><b>ContextUser</b></dt>
</dl>
</td>
<td width="60%">
The certificate is intended for an end user.

</td>
</tr>
<tr>
<td width="40%"><a id="ContextMachine"></a><a id="contextmachine"></a><a id="CONTEXTMACHINE"></a><dl>
<dt><b>ContextMachine</b></dt>
</dl>
</td>
<td width="60%">
The certificate is intended for a computer.

</td>
</tr>
<tr>
<td width="40%"><a id="ContextAdministratorForceMachine"></a><a id="contextadministratorforcemachine"></a><a id="CONTEXTADMINISTRATORFORCEMACHINE"></a><dl>
<dt><b>ContextAdministratorForceMachine</b></dt>
</dl>
</td>
<td width="60%">
The certificate is being requested by an administrator acting on the behalf of a computer.

</td>
</tr>
</table>
 


## -returns



If the function succeeds, the function returns <b>S_OK</b>.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following table.  For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>HRESULT_FROM_WIN32(ERROR_ALREADY_INITIALIZED</b></dt>
</dl>
</td>
<td width="60%">
The object has already been initialized.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/19124591-be1a-401e-9b83-c640d00de34a">IX509EnrollmentHelper</a>
 

 

