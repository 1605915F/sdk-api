---
UID: NN:xpsdigitalsignature.IXpsSignatureBlockCollection
title: IXpsSignatureBlockCollection (xpsdigitalsignature.h)
author: windows-sdk-content
description: A collection of IXpsSignatureBlock interfaces.
old-location: xps\ixpssignatureblockcollection.htm
tech.root: printdocs
ms.assetid: e8f7be84-389e-40cf-a093-83417ba184c7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IXpsSignatureBlockCollection, IXpsSignatureBlockCollection interface [XPS Documents and Packaging], IXpsSignatureBlockCollection interface [XPS Documents and Packaging],described, xps.ixpssignatureblockcollection, xpsdigitalsignature/IXpsSignatureBlockCollection
ms.topic: interface
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
 - IXpsSignatureBlockCollection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsSignatureBlockCollection interface


## -description


A collection of <a href="https://msdn.microsoft.com/cb2b7fe2-f3d9-4542-958f-5412d2498a9f">IXpsSignatureBlock</a> interfaces.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IXpsSignatureBlockCollection</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IXpsSignatureBlockCollection</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IXpsSignatureBlockCollection</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4d3f89be-f9f3-46db-802f-ffb4867786c2">GetAt</a>
</td>
<td align="left" width="63%">
Gets an <a href="https://msdn.microsoft.com/cb2b7fe2-f3d9-4542-958f-5412d2498a9f">IXpsSignatureBlock</a> interface pointer from a specified location in the collection.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d748e974-7350-44cd-9599-111f402d20e2">GetCount</a>
</td>
<td align="left" width="63%">
Gets the number of <a href="https://msdn.microsoft.com/cb2b7fe2-f3d9-4542-958f-5412d2498a9f">IXpsSignatureBlock</a> interface pointers in the collection.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/895f6f0b-6259-4288-90be-659f1ca46d1a">RemoveAt</a>
</td>
<td align="left" width="63%">
Removes and releases an <a href="https://msdn.microsoft.com/cb2b7fe2-f3d9-4542-958f-5412d2498a9f">IXpsSignatureBlock</a> interface pointer from a specified location in the collection.
            

</td>
</tr>
</table> 


## -remarks



This interface cannot exist independently from the signature manager from which it was instantiated.

For more information about the collection methods, see  <a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>.




## -see-also




<a href="https://msdn.microsoft.com/cb2b7fe2-f3d9-4542-958f-5412d2498a9f">IXpsSignatureBlock</a>



<a href="https://msdn.microsoft.com/8d72ff28-6dfb-4fa8-a1b6-14b054aa7eb5">Interfaces</a>



<a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>
 

 

