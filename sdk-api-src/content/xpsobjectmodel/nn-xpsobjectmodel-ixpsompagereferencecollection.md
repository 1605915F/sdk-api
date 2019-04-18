---
UID: NN:xpsobjectmodel.IXpsOMPageReferenceCollection
title: IXpsOMPageReferenceCollection (xpsobjectmodel.h)
author: windows-sdk-content
description: A collection of IXpsOMPageReference interface pointers.
old-location: xps\ixpsompagereferencecollection.htm
tech.root: printdocs
ms.assetid: 4b51bc29-c653-41fa-bbd3-9ff529f84e4e
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IXpsOMPageReferenceCollection, IXpsOMPageReferenceCollection interface [XPS Documents and Packaging], IXpsOMPageReferenceCollection interface [XPS Documents and Packaging],described, xps.ixpsompagereferencecollection, xpsobjectmodel/IXpsOMPageReferenceCollection
ms.topic: interface
req.header: xpsobjectmodel.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: XpsObjectModel.idl
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
 - xpsobjectmodel.h
api_name:
 - IXpsOMPageReferenceCollection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IXpsOMPageReferenceCollection interface


## -description


A collection of <a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a> interface pointers.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IXpsOMPageReferenceCollection</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IXpsOMPageReferenceCollection</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IXpsOMPageReferenceCollection</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/89fce79b-9211-4e47-884c-11c98718570e">Append</a>
</td>
<td align="left" width="63%">
Appends an <a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a> interface to the end of the collection.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5b888771-fc69-4857-94a4-eea5a068c740">GetAt</a>
</td>
<td align="left" width="63%">
Gets an <a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a> interface pointer from a specified location in the collection.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7728930a-408d-445f-9b0d-9043912d4e72">GetCount</a>
</td>
<td align="left" width="63%">
Gets the number of <a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a> interface pointers in the collection.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/829d0b81-90e2-4051-a9a7-7f71602f8c13">InsertAt</a>
</td>
<td align="left" width="63%">
Inserts an <a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a> interface pointer at a specified location in the collection.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/905ed1ea-b694-4620-8a71-2f0bfb831af4">RemoveAt</a>
</td>
<td align="left" width="63%">
Removes and releases an <a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a> interface pointer from a specified location in the collection.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b06b7ae2-e684-46a3-ab46-9f33cc6c10fc">SetAt</a>
</td>
<td align="left" width="63%">
Replaces an <a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a> interface pointer at a specified location in the collection.
            

</td>
</tr>
</table> 


## -remarks



For more information about the collection methods, see <a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>.




## -see-also




<a href="https://msdn.microsoft.com/cdebab24-f918-4235-b4d5-5ee1007ade87">IXpsOMPageReference</a>



<a href="https://msdn.microsoft.com/8d72ff28-6dfb-4fa8-a1b6-14b054aa7eb5">Interfaces</a>



<a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>
 

 

