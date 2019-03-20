---
UID: NF:msopc.IOpcDigitalSignature.GetCanonicalizationMethod
title: IOpcDigitalSignature::GetCanonicalizationMethod (msopc.h)
author: windows-sdk-content
description: Gets the canonicalization method that was applied to the SignedInfo element of the serialized signature.
old-location: opc\iopcdigitalsignature_getcanonicalizationmethod.htm
tech.root: OPC
ms.assetid: 59c89909-6e35-4210-b76c-c820a9bb0d8e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetCanonicalizationMethod, GetCanonicalizationMethod method [Open Packaging Conventions], GetCanonicalizationMethod method [Open Packaging Conventions],IOpcDigitalSignature interface, IOpcDigitalSignature interface [Open Packaging Conventions],GetCanonicalizationMethod method, IOpcDigitalSignature.GetCanonicalizationMethod, IOpcDigitalSignature::GetCanonicalizationMethod, msopc/IOpcDigitalSignature::GetCanonicalizationMethod, opc.iopcdigitalsignature_getcanonicalizationmethod
ms.topic: method
req.header: msopc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OpcDigitalSignature.idl
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
 - msopc.h
api_name:
 - IOpcDigitalSignature.GetCanonicalizationMethod
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOpcDigitalSignature::GetCanonicalizationMethod


## -description


Gets the canonicalization method  that was applied to the <b>SignedInfo</b> element of the serialized signature.


## -parameters




### -param canonicalizationMethod [out, retval]

An <a href="https://msdn.microsoft.com/f8401d12-da2e-4b35-b473-ebe3d1f91abd">OPC_CANONICALIZATION_METHOD</a>  value that specifies the canonicalization method that was applied to the <b>SignedInfo</b> element of the signature markup when the signature was generated.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>canonicalizationMethod</i> parameter is <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



When using the APIs to generate a signature, the C14N canonicalization method that removes comments is applied to the <b>SignedInfo</b> element. This method corresponds to the <b>OPC_CANONICALIZATION_C14N</b> enum value.


#### Thread Safety

Packaging objects are not thread-safe.

For more information, see the <a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>.




## -see-also




<a href="https://msdn.microsoft.com/62069595-0d1e-44e5-b68d-2bb0c355c565">Core Packaging Interfaces</a>



<a href="https://msdn.microsoft.com/d81f6569-6c95-4bb7-9d1d-51e10701b970">Digital Signatures Overview</a>



<a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>



<a href="https://msdn.microsoft.com/cfa38ef6-9d96-4577-a3bf-518784d19ad8">IOpcDigitalSignature</a>



<b>Overviews</b>



<a href="https://msdn.microsoft.com/cb35d87e-bbec-42d3-9f9d-d1cf36f39419">Packaging API Programming Guide</a>



<a href="https://msdn.microsoft.com/7ab1cc09-ce81-4f56-8adf-d8c95bf2c4cd">Packaging API Reference</a>



<a href="https://msdn.microsoft.com/885137be-35d5-4ec5-bbcc-16c95adf55ab">Packaging API Samples</a>



<a href="https://msdn.microsoft.com/76455a88-81be-45d9-a682-2ba43038b43f">Packaging Digital Signature Interfaces</a>



<a href="https://msdn.microsoft.com/a0e9f38f-ab35-4fc2-855c-ea21bf164223">Packaging Interfaces</a>



<b>Reference</b>
 

 

