---
UID: NF:msopc.IOpcSignatureRelationshipReferenceEnumerator.MovePrevious
title: IOpcSignatureRelationshipReferenceEnumerator::MovePrevious (msopc.h)
author: windows-sdk-content
description: Moves the current position of the enumerator to the previous IOpcSignatureRelationshipReference interface pointer.
old-location: opc\iopcsignaturerelationshipreferenceenumerator_moveprevious.htm
tech.root: OPC
ms.assetid: c56f871f-50ca-4253-84db-0602459fc2fa
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOpcSignatureRelationshipReferenceEnumerator interface [Open Packaging Conventions],MovePrevious method, IOpcSignatureRelationshipReferenceEnumerator.MovePrevious, IOpcSignatureRelationshipReferenceEnumerator::MovePrevious, MovePrevious, MovePrevious method [Open Packaging Conventions], MovePrevious method [Open Packaging Conventions],IOpcSignatureRelationshipReferenceEnumerator interface, msopc/IOpcSignatureRelationshipReferenceEnumerator::MovePrevious, opc.iopcsignaturerelationshipreferenceenumerator_moveprevious
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
 - IOpcSignatureRelationshipReferenceEnumerator.MovePrevious
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOpcSignatureRelationshipReferenceEnumerator::MovePrevious


## -description


Moves the current position of the enumerator to the previous <a href="https://msdn.microsoft.com/24aebfff-6b4f-49cb-988f-670ffed7d815">IOpcSignatureRelationshipReference</a> interface pointer.


## -parameters




### -param hasPrevious [out, retval]

A Boolean value that indicates the status of the <a href="https://msdn.microsoft.com/24aebfff-6b4f-49cb-988f-670ffed7d815">IOpcSignatureRelationshipReference</a> interface pointer at the current position.

The value of <i>hasPrevious</i> is only valid when the method succeeds.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>TRUE</dt>
</dl>
</td>
<td width="60%">
The current position of the enumerator has been moved to the previous pointer in the collection, and that pointer is valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>FALSE</dt>
</dl>
</td>
<td width="60%">
The current position of the enumerator has been moved past the beginning of the collection and is no longer valid.

</td>
</tr>
</table>
 


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
The <i>hasPrevious</i> parameter is <b>NULL</b>.

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
<tr>
<td width="40%">
<dl>
<dt><b>OPC_E_ENUM_CANNOT_MOVE_PREVIOUS</b></dt>
<dt>0x80510052</dt>
</dl>
</td>
<td width="60%">
The current position already precedes the first item of the enumerator.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/62069595-0d1e-44e5-b68d-2bb0c355c565">Core Packaging Interfaces</a>



<a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>



<a href="https://msdn.microsoft.com/aa4c6e8b-1a1f-464b-885e-bee0976afafc">IOpcSignatureRelationshipReferenceEnumerator</a>



<b>Overviews</b>



<a href="https://msdn.microsoft.com/cb35d87e-bbec-42d3-9f9d-d1cf36f39419">Packaging API Programming Guide</a>



<a href="https://msdn.microsoft.com/7ab1cc09-ce81-4f56-8adf-d8c95bf2c4cd">Packaging API Reference</a>



<a href="https://msdn.microsoft.com/885137be-35d5-4ec5-bbcc-16c95adf55ab">Packaging API Samples</a>



<a href="https://msdn.microsoft.com/76455a88-81be-45d9-a682-2ba43038b43f">Packaging Digital Signature Interfaces</a>



<a href="https://msdn.microsoft.com/a0e9f38f-ab35-4fc2-855c-ea21bf164223">Packaging Interfaces</a>



<b>Reference</b>
 

 

