---
UID: NF:xpsobjectmodel.IXpsOMSignatureBlockResourceCollection.SetAt
title: IXpsOMSignatureBlockResourceCollection::SetAt
author: windows-sdk-content
description: Replaces an IXpsOMSignatureBlockResource interface pointer at a specified location in the collection.
old-location: xps\ixpsomsignatureblockresourcecollection_setat.htm
tech.root: printdocs
ms.assetid: c1f88493-0f81-4aac-b6d6-049d10934254
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IXpsOMSignatureBlockResourceCollection interface [XPS Documents and Packaging],SetAt method, IXpsOMSignatureBlockResourceCollection.SetAt, IXpsOMSignatureBlockResourceCollection::SetAt, SetAt, SetAt method [XPS Documents and Packaging], SetAt method [XPS Documents and Packaging],IXpsOMSignatureBlockResourceCollection interface, xps.ixpsomsignatureblockresourcecollection_setat, xpsobjectmodel/IXpsOMSignatureBlockResourceCollection::SetAt
ms.topic: method
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
 - IXpsOMSignatureBlockResourceCollection.SetAt
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMSignatureBlockResourceCollection::SetAt


## -description


Replaces an <a href="https://msdn.microsoft.com/f5052470-487d-4f47-8d42-70538a4a45a8">IXpsOMSignatureBlockResource</a> interface pointer at a specified location in the collection.


## -parameters




### -param index [in]

The zero-based index in the collection where an <a href="https://msdn.microsoft.com/f5052470-487d-4f47-8d42-70538a4a45a8">IXpsOMSignatureBlockResource</a> interface pointer is to be replaced.


### -param signatureBlockResource [in]

The <a href="https://msdn.microsoft.com/f5052470-487d-4f47-8d42-70538a4a45a8">IXpsOMSignatureBlockResource</a> interface pointer that will replace current contents at the location specified by <i>index</i>.


## -returns



If the method succeeds, it returns S_OK; otherwise, it returns an <b>HRESULT</b> error code.




## -remarks



At the location specified by <i>index</i>, this method releases the <a href="https://msdn.microsoft.com/f5052470-487d-4f47-8d42-70538a4a45a8">IXpsOMSignatureBlockResource</a> interface referenced by the existing pointer, then writes the pointer  that is passed in <i>signatureBlockResource</i>.

For more information about the collection methods, see  <a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>.




## -see-also




<a href="https://msdn.microsoft.com/f5052470-487d-4f47-8d42-70538a4a45a8">IXpsOMSignatureBlockResource</a>



<a href="https://msdn.microsoft.com/681bdb9c-69dd-4bf6-a4b3-c490f7a0363e">IXpsOMSignatureBlockResourceCollection</a>



<a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>
 

 

