---
UID: NF:xpsdigitalsignature.IXpsSignatureBlock.GetRequests
title: IXpsSignatureBlock::GetRequests (xpsdigitalsignature.h)
author: windows-sdk-content
description: Gets a pointer to the IXpsSignatureRequestCollection interface that contains a collection of signature requests.
old-location: xps\ixpssignatureblock_getrequests.htm
tech.root: printdocs
ms.assetid: 97050917-8b41-4e4f-80c5-d8f166897c96
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetRequests, GetRequests method [XPS Documents and Packaging], GetRequests method [XPS Documents and Packaging],IXpsSignatureBlock interface, IXpsSignatureBlock interface [XPS Documents and Packaging],GetRequests method, IXpsSignatureBlock.GetRequests, IXpsSignatureBlock::GetRequests, xps.ixpssignatureblock_getrequests, xpsdigitalsignature/IXpsSignatureBlock::GetRequests
ms.topic: method
req.header: xpsdigitalsignature.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: XpsDigitalSignature.idl
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
 - xpsdigitalsignature.h
api_name:
 - IXpsSignatureBlock.GetRequests
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IXpsSignatureBlock::GetRequests


## -description


Gets a pointer to the <a href="https://msdn.microsoft.com/bb8279e1-a98b-4156-8b90-d9b69411bfa3">IXpsSignatureRequestCollection</a> interface that contains a collection of signature requests.


## -parameters




### -param requests [out, retval]

A pointer to the <a href="https://msdn.microsoft.com/bb8279e1-a98b-4156-8b90-d9b69411bfa3">IXpsSignatureRequestCollection</a> interface that contains a collection of signature requests.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the table that follows. For return values that are not listed in this table, see <a href="https://msdn.microsoft.com/d20707b0-55ea-438a-8ce3-972c61678928">XPS Digital Signature API Errors</a> and  <a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>.

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
<i>requests</i> is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
 The interface is not connected to the signature manager.

</td>
</tr>
</table>
 




## -remarks



Signature requests are added to the  collection of signature requests  by parsing the XML markup 
    of the corresponding SignatureDefinitions part while <a href="https://msdn.microsoft.com/ecb33eee-4622-4a2e-bc24-7a77d16ef4a4">LoadPackageFile</a> or <a href="https://msdn.microsoft.com/755bbd41-0941-4956-a99d-45b39f9b030f">LoadPackageStream</a> reads the XPS package.




## -see-also




<a href="https://msdn.microsoft.com/cb2b7fe2-f3d9-4542-958f-5412d2498a9f">IXpsSignatureBlock</a>



<a href="https://msdn.microsoft.com/31283ebe-91f4-42be-9a9b-6fcd641dc356">IXpsSignatureManager</a>



<a href="https://msdn.microsoft.com/bb8279e1-a98b-4156-8b90-d9b69411bfa3">IXpsSignatureRequestCollection</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>



<a href="https://msdn.microsoft.com/d20707b0-55ea-438a-8ce3-972c61678928">XPS Digital Signature API Errors</a>



<a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>
 

 

