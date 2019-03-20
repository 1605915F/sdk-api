---
UID: NF:msopc.IOpcDigitalSignatureEnumerator.Clone
title: IOpcDigitalSignatureEnumerator::Clone (msopc.h)
author: windows-sdk-content
description: Creates a copy of the current IOpcDigitalSignatureEnumerator interface pointer and all its descendants.
old-location: opc\iopcdigitalsignatureenumerator_clone.htm
tech.root: OPC
ms.assetid: f7a544b6-6c2d-40ce-9148-63780cbbf44f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Clone, Clone method [Open Packaging Conventions], Clone method [Open Packaging Conventions],IOpcDigitalSignatureEnumerator interface, IOpcDigitalSignatureEnumerator interface [Open Packaging Conventions],Clone method, IOpcDigitalSignatureEnumerator.Clone, IOpcDigitalSignatureEnumerator::Clone, msopc/IOpcDigitalSignatureEnumerator::Clone, opc.iopcdigitalsignatureenumerator_clone
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
 - IOpcDigitalSignatureEnumerator.Clone
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOpcDigitalSignatureEnumerator::Clone


## -description


Creates a copy of the current <a href="https://msdn.microsoft.com/73fd0e47-7503-470d-b649-e4b2ba492bf1">IOpcDigitalSignatureEnumerator</a> interface pointer and all its descendants.


## -parameters




### -param copy [out, retval]

A pointer to a copy of the <a href="https://msdn.microsoft.com/73fd0e47-7503-470d-b649-e4b2ba492bf1">IOpcDigitalSignatureEnumerator</a> interface pointer.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code/value</th>
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
The <i>copy</i> parameter is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>OPC_E_ENUM_COLLECTION_CHANGED</b></dt>
<dt>0x80510050</dt>
</dl>
</td>
<td width="60%">
The enumerator is invalid because the underlying set has changed.

</td>
</tr>
</table>
 




## -remarks



The copy has a current position  and set that are identical to the current enumerator.


#### Thread Safety

Packaging objects are not thread-safe.

For more information, see the <a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>.




## -see-also




<a href="https://msdn.microsoft.com/d81f6569-6c95-4bb7-9d1d-51e10701b970">Digital Signatures Overview</a>



<a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>



<a href="https://msdn.microsoft.com/73fd0e47-7503-470d-b649-e4b2ba492bf1">IOpcDigitalSignatureEnumerator</a>



<b>Overviews</b>



<a href="https://msdn.microsoft.com/cb35d87e-bbec-42d3-9f9d-d1cf36f39419">Packaging API Programming Guide</a>



<a href="https://msdn.microsoft.com/7ab1cc09-ce81-4f56-8adf-d8c95bf2c4cd">Packaging API Reference</a>



<a href="https://msdn.microsoft.com/885137be-35d5-4ec5-bbcc-16c95adf55ab">Packaging API Samples</a>



<a href="https://msdn.microsoft.com/76455a88-81be-45d9-a682-2ba43038b43f">Packaging Digital Signature Interfaces</a>



<a href="https://msdn.microsoft.com/a0e9f38f-ab35-4fc2-855c-ea21bf164223">Packaging Interfaces</a>



<b>Reference</b>
 

 

