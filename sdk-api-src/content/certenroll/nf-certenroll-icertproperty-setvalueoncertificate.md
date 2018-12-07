---
UID: NF:certenroll.ICertProperty.SetValueOnCertificate
title: ICertProperty::SetValueOnCertificate
author: windows-sdk-content
description: Associates a property value with an existing certificate.
old-location: security\icertproperty_setvalueoncertificate_method.htm
tech.root: seccertenroll
ms.assetid: 46c409c4-46bd-4349-8363-1983f4411bc2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICertProperty interface [Security],SetValueOnCertificate method, ICertProperty.SetValueOnCertificate, ICertProperty::SetValueOnCertificate, SetValueOnCertificate, SetValueOnCertificate method [Security], SetValueOnCertificate method [Security],ICertProperty interface, certenroll/ICertProperty::SetValueOnCertificate, security.icertproperty_setvalueoncertificate_method
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ICertProperty.SetValueOnCertificate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICertProperty::SetValueOnCertificate


## -description


The <b>SetValueOnCertificate</b> method associates a property value with an existing certificate.


## -parameters




### -param MachineContext [in]

A <b>VARIANT_BOOL</b> value that indicates  whether the certificate store is for the local computer or the current user. Specify <b>VARIANT_TRUE</b> for the computer and <b>VARIANT_FALSE</b> for the user.


### -param Encoding [in]

An <a href="https://msdn.microsoft.com/en-us/library/Aa374936(v=VS.85).aspx">EncodingType</a> enumeration value that specifies the type of Unicode encoding applied to  the certificate string identified by the <i>strCertificate</i> parameter.


### -param strCertificate [in]

A <b>BSTR</b> variable that contains the DER-encoded certificate.

Beginning with Windows 7 and Windows Server 2008 R2, you can specify a certificate thumb print or serial number rather than an encoded certificate. Doing so causes the function to search the appropriate local stores for the matching certificate. Keep in mind the following points:

<ul>
<li>The <b>BSTR</b> must be an even number of hexadecimal digits.</li>
<li>Whitespace between hexadecimal pairs is ignored.</li>
<li>The <i>Encoding</i> parameter must be set to <b>XCN_CRYPT_STRING_HEXRAW</b>.</li>
<li>The <i>MachineContext</i> parameter determines whether the user or computer stores or both are searched.</li>
<li>If a private key is needed, only the personal and request stores are searched.</li>
<li>If a private key is not needed, the root and intermediate CA stores are also searched.</li>
</ul>

## -returns



If the function succeeds, the function returns <b>S_OK</b>.

If the function fails, it returns an <b>HRESULT</b> value that indicates the error. Possible values include, but are not limited to, those in the following table. For a list of common error codes, see <a href="https://msdn.microsoft.com/en-us/library/Aa378137(v=VS.85).aspx">Common HRESULT Values</a>.

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>CRYPT_E_NOT_FOUND</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The certificate could not be found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b><b>CRYPT_E_UNEXPECTED_MSG_TYPE</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The certificate was found but the private key could not be loaded.

</td>
</tr>
</table>
 




## -remarks



Call the <a href="https://msdn.microsoft.com/en-us/library/Aa375811(v=VS.85).aspx">InitializeDecode</a> method or the <a href="https://msdn.microsoft.com/en-us/library/Aa375817(v=VS.85).aspx">InitializeFromCertificate</a> method to create a property value. Before calling either method, you must first set the <a href="https://msdn.microsoft.com/en-us/library/Aa375830(v=VS.85).aspx">PropertyId</a> property to specify which property value to initialize.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa375231(v=VS.85).aspx">ICertProperties</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa375239(v=VS.85).aspx">ICertProperty</a>
 

 

