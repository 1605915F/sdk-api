---
UID: NF:certenroll.IX509ExtensionSubjectKeyIdentifier.InitializeDecode
title: IX509ExtensionSubjectKeyIdentifier::InitializeDecode
author: windows-sdk-content
description: Initializes the extension from a Distinguished Encoding Rules (DER) encoded byte array that contains the extension value.
old-location: security\ix509extensionsubjectkeyidentifier_initializedecode_method.htm
tech.root: seccertenroll
ms.assetid: 5886187d-33b1-4151-a01f-de263c41c27b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IX509ExtensionSubjectKeyIdentifier interface [Security],InitializeDecode method, IX509ExtensionSubjectKeyIdentifier.InitializeDecode, IX509ExtensionSubjectKeyIdentifier::InitializeDecode, InitializeDecode, InitializeDecode method [Security], InitializeDecode method [Security],IX509ExtensionSubjectKeyIdentifier interface, certenroll/IX509ExtensionSubjectKeyIdentifier::InitializeDecode, security.ix509extensionsubjectkeyidentifier_initializedecode_method
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
 - IX509ExtensionSubjectKeyIdentifier.InitializeDecode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IX509ExtensionSubjectKeyIdentifier::InitializeDecode


## -description


The <b>InitializeDecode</b> method initializes the  extension from a <a href="https://msdn.microsoft.com/en-us/library/ms721573(v=VS.85).aspx">Distinguished Encoding Rules</a> (DER) encoded byte array that contains the extension value. The encoded byte array is represented by a Unicode encoded string.


## -parameters




### -param Encoding [in]

An <a href="https://msdn.microsoft.com/en-us/library/Aa374936(v=VS.85).aspx">EncodingType</a> enumeration value that specifies the type of Unicode encoding applied to  the <i>strEncodedData</i> parameter.


### -param strEncodedData [in]

A <b>BSTR</b> variable that contains the DER-encoded extension.


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
<dt><b><b>HRESULT_FROM_WIN32(ERROR_ALREADY_INITIALIZED)</b></b></dt>
<dt></dt>
</dl>
</td>
<td width="60%">
The object is already initialized.

</td>
</tr>
</table>
 




## -remarks



You can use this method if you have a DER-encoded <a href="https://msdn.microsoft.com/en-us/library/ms721532(v=VS.85).aspx">Abstract Syntax Notation One</a> (ASN.1) object that contains a <b>SubjectKeyIdentifier</b> extension.  You must supply the DER-encoded object in a Unicode encoded string. For more information, see the <a href="https://msdn.microsoft.com/en-us/library/Aa375047(v=VS.85).aspx">IBinaryConverter</a> interface.

You must call either <a href="https://msdn.microsoft.com/en-us/library/Aa378220(v=VS.85).aspx">InitializeEncode</a> or <b>InitializeDecode</b> before you can use an  <a href="https://msdn.microsoft.com/en-us/library/Aa378215(v=VS.85).aspx">IX509ExtensionSubjectKeyIdentifier</a> object. The two methods complement each other. The <b>InitializeEncode</b> method enables you to construct a DER-encoded ASN.1 extension object from raw data, and the <b>InitializeDecode</b> method enables you to initialize the raw data from an encoded object.

You can retrieve the following properties for this extension:<ul>
<li>The <a href="https://msdn.microsoft.com/en-us/library/Aa378409(v=VS.85).aspx">Critical</a> property identifies whether the extension is critical. You can also specify this property.</li>
<li>The <a href="https://msdn.microsoft.com/en-us/library/Aa378518(v=VS.85).aspx">ObjectId</a> property retrieves the <a href="https://msdn.microsoft.com/en-us/library/ms721599(v=VS.85).aspx">object identifier</a> (OID).</li>
<li>The <a href="https://msdn.microsoft.com/en-us/library/Aa378236(v=VS.85).aspx">SubjectKeyIdentifier</a> property retrieves the raw data.</li>
</ul>





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa378215(v=VS.85).aspx">IX509ExtensionSubjectKeyIdentifier</a>
 

 

