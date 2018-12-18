---
UID: NF:certenroll.ICspInformation.GetDefaultSecurityDescriptor
title: ICspInformation::GetDefaultSecurityDescriptor
author: windows-sdk-content
description: Retrieves the default private key security descriptor.
old-location: security\icspinformation_getdefaultsecuritydescriptor.htm
tech.root: seccertenroll
ms.assetid: b4594400-29f2-47e2-8b4f-87ee82ea5e82
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDefaultSecurityDescriptor, GetDefaultSecurityDescriptor method [Security], GetDefaultSecurityDescriptor method [Security],ICspInformation interface, ICspInformation interface [Security],GetDefaultSecurityDescriptor method, ICspInformation.GetDefaultSecurityDescriptor, ICspInformation::GetDefaultSecurityDescriptor, certenroll/ICspInformation::GetDefaultSecurityDescriptor, security.icspinformation_getdefaultsecuritydescriptor
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
 - ICspInformation.GetDefaultSecurityDescriptor
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICspInformation::GetDefaultSecurityDescriptor


## -description


The <b>GetDefaultSecurityDescriptor</b> method retrieves the default private key security descriptor.


## -parameters




### -param MachineContext [in]

A <b>VARIANT_BOOL</b> variable that indicates whether to retrieve the security descriptor for the computer or the user. Specify <b>VARIANT_TRUE</b> for the computer and <b>VARIANT_FALSE</b> for the user.


### -param pValue [out]

Pointer to a  <b>BSTR</b> variable that contains the security descriptor.


## -returns



If the function succeeds, the function returns <b>S_OK</b>.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following table. For a list of common error codes, see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>CERTSRV_E_PROPERTY_EMPTY</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The property value could not be found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>NTE_BAD_TYPE</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The cryptographic provider does not support security descriptors.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>NTE_NOT_FOUND</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The cryptographic provider does not support security descriptors.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>NTE_BAD_KEY_STATE</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The cryptographic provider does not support security descriptors.

</td>
</tr>
</table>
 




## -remarks



To use the security descriptor, you must call the <a href="https://msdn.microsoft.com/c5654148-fb4c-436d-9378-a1168fc82607">ConvertStringSecurityDescriptorToSecurityDescriptor</a> function included with the Microsoft Authorization API and specify the string returned by the <b>GetDefaultSecurityDescriptor</b> method. The function returns a pointer to a <a href="https://msdn.microsoft.com/653992aa-4e32-4187-b3ac-727e82bfe0b6">SECURITY_DESCRIPTOR</a> structure.

The default security descriptor is used to define access to private keys for the computer and user in the following manner:<ul>
<li>By default, only local administrators and services running under the LocalSystem account can access private keys associated with the computer account.</li>
<li>When a provider stores the private key of a user in an encrypted file in the user profile, it uses a security descriptor to set access permissions to the file.</li>
</ul>


This method retrieves the default security descriptor that will be associated with the specified <i>MachineContext</i> parameter and the current provider if a new private key is created.  You can use the default descriptor to create a custom descriptor. Custom descriptors are typically created when a private key associated with a computer context certificate must be used by a service running under an account other than the LocalSystem account.

Some cryptographic providers do not support security descriptors. Examples include smart card and hardware security module (HSM) providers.




## -see-also




<a href="https://msdn.microsoft.com/e337ae2c-6f86-4025-8d31-47bc5d8a4ca8">ICspInformation</a>
 

 

