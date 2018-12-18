---
UID: NF:msopc.IOpcSignatureRelationshipReferenceSet.GetEnumerator
title: IOpcSignatureRelationshipReferenceSet::GetEnumerator
author: windows-sdk-content
description: Gets an enumerator of IOpcSignatureRelationshipReference interface pointers in the set.
old-location: opc\iopcsignaturerelationshipreferenceset_getenumerator.htm
tech.root: OPC
ms.assetid: a574a935-f89a-445f-a793-d8dc2e116a48
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetEnumerator, GetEnumerator method [Open Packaging Conventions], GetEnumerator method [Open Packaging Conventions],IOpcSignatureRelationshipReferenceSet interface, IOpcSignatureRelationshipReferenceSet interface [Open Packaging Conventions],GetEnumerator method, IOpcSignatureRelationshipReferenceSet.GetEnumerator, IOpcSignatureRelationshipReferenceSet::GetEnumerator, msopc/IOpcSignatureRelationshipReferenceSet::GetEnumerator, opc.iopcsignaturerelationshipreferenceset_getenumerator
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
 - IOpcSignatureRelationshipReferenceSet.GetEnumerator
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOpcSignatureRelationshipReferenceSet::GetEnumerator


## -description


Gets an enumerator of <a href="https://msdn.microsoft.com/24aebfff-6b4f-49cb-988f-670ffed7d815">IOpcSignatureRelationshipReference</a> interface pointers in the set.


## -parameters




### -param relationshipReferenceEnumerator [out, retval]

A pointer to an enumerator of <a href="https://msdn.microsoft.com/24aebfff-6b4f-49cb-988f-670ffed7d815">IOpcSignatureRelationshipReference</a> interface pointers in the set.


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
The <i>relationshipReferenceEnumerator</i> parameter is <b>NULL</b>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/62069595-0d1e-44e5-b68d-2bb0c355c565">Core Packaging Interfaces</a>



<a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>



<a href="https://msdn.microsoft.com/aa4c6e8b-1a1f-464b-885e-bee0976afafc">IOpcSignatureRelationshipReferenceEnumerator</a>



<a href="https://msdn.microsoft.com/89ea7243-54ee-487b-a58a-0721af9db8c3">IOpcSignatureRelationshipReferenceSet</a>



<b>Overviews</b>



<a href="https://msdn.microsoft.com/cb35d87e-bbec-42d3-9f9d-d1cf36f39419">Packaging API Programming Guide</a>



<a href="https://msdn.microsoft.com/7ab1cc09-ce81-4f56-8adf-d8c95bf2c4cd">Packaging API Reference</a>



<a href="https://msdn.microsoft.com/885137be-35d5-4ec5-bbcc-16c95adf55ab">Packaging API Samples</a>



<a href="https://msdn.microsoft.com/76455a88-81be-45d9-a682-2ba43038b43f">Packaging Digital Signature Interfaces</a>



<a href="https://msdn.microsoft.com/a0e9f38f-ab35-4fc2-855c-ea21bf164223">Packaging Interfaces</a>



<b>Reference</b>
 

 

