---
UID: NF:msopc.IOpcSignatureRelationshipReference.GetRelationshipSigningOption
title: IOpcSignatureRelationshipReference::GetRelationshipSigningOption (msopc.h)
author: windows-sdk-content
description: Gets a value that describes whether all or a subset of relationships that are stored in the referenced&#160;Relationships part are selected.
old-location: opc\iopcsignaturerelationshipreference_getrelationshipsigningoption.htm
tech.root: OPC
ms.assetid: 9960c67c-4f09-435e-b82c-ca449645f6e5
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRelationshipSigningOption, GetRelationshipSigningOption method [Open Packaging Conventions], GetRelationshipSigningOption method [Open Packaging Conventions],IOpcSignatureRelationshipReference interface, IOpcSignatureRelationshipReference interface [Open Packaging Conventions],GetRelationshipSigningOption method, IOpcSignatureRelationshipReference.GetRelationshipSigningOption, IOpcSignatureRelationshipReference::GetRelationshipSigningOption, msopc/IOpcSignatureRelationshipReference::GetRelationshipSigningOption, opc.iopcsignaturerelationshipreference_getrelationshipsigningoption
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
 - IOpcSignatureRelationshipReference.GetRelationshipSigningOption
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOpcSignatureRelationshipReference::GetRelationshipSigningOption


## -description


Gets a value that describes whether all or a subset of relationships that are stored in the referenced Relationships part are selected.


## -parameters




### -param relationshipSigningOption [out, retval]

A value that describes whether all or a subset of relationships are selected.


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
The <i>relationshipSigningOption</i> parameter is <b>NULL</b>.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/62069595-0d1e-44e5-b68d-2bb0c355c565">Core Packaging Interfaces</a>



<a href="https://msdn.microsoft.com/ef392c88-49cd-4ffa-b1fb-1501c6448264">Getting Started with the Packaging API</a>



<a href="https://msdn.microsoft.com/24aebfff-6b4f-49cb-988f-670ffed7d815">IOpcSignatureRelationshipReference</a>



<a href="https://msdn.microsoft.com/b6a83730-459a-4119-a013-7d670e659c32">OPC_RELATIONSHIPS_SIGNING_OPTION</a>



<b>Overviews</b>



<a href="https://msdn.microsoft.com/cb35d87e-bbec-42d3-9f9d-d1cf36f39419">Packaging API Programming Guide</a>



<a href="https://msdn.microsoft.com/7ab1cc09-ce81-4f56-8adf-d8c95bf2c4cd">Packaging API Reference</a>



<a href="https://msdn.microsoft.com/885137be-35d5-4ec5-bbcc-16c95adf55ab">Packaging API Samples</a>



<a href="https://msdn.microsoft.com/76455a88-81be-45d9-a682-2ba43038b43f">Packaging Digital Signature Interfaces</a>



<a href="https://msdn.microsoft.com/a0e9f38f-ab35-4fc2-855c-ea21bf164223">Packaging Interfaces</a>



<b>Reference</b>
 

 

