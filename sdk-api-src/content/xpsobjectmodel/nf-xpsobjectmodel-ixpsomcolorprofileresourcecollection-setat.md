---
UID: NF:xpsobjectmodel.IXpsOMColorProfileResourceCollection.SetAt
title: IXpsOMColorProfileResourceCollection::SetAt
author: windows-sdk-content
description: Replaces an IXpsOMColorProfileResource interface pointer at a specified location in the collection.
old-location: xps\ixpsomcolorprofileresourcecollection_setat.htm
tech.root: printdocs
ms.assetid: dbabddbb-a558-4166-9951-7126221d88e6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IXpsOMColorProfileResourceCollection interface [XPS Documents and Packaging],SetAt method, IXpsOMColorProfileResourceCollection.SetAt, IXpsOMColorProfileResourceCollection::SetAt, SetAt, SetAt method [XPS Documents and Packaging], SetAt method [XPS Documents and Packaging],IXpsOMColorProfileResourceCollection interface, xps.ixpsomcolorprofileresourcecollection_setat, xpsobjectmodel/IXpsOMColorProfileResourceCollection::SetAt
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
 - IXpsOMColorProfileResourceCollection.SetAt
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMColorProfileResourceCollection::SetAt


## -description


Replaces an <a href="https://msdn.microsoft.com/8a344300-c3fc-4225-bfa5-d5d33798a094">IXpsOMColorProfileResource</a> interface pointer at a specified location in the collection.


## -parameters




### -param index [in]

The zero-based index in the collection where an <a href="https://msdn.microsoft.com/8a344300-c3fc-4225-bfa5-d5d33798a094">IXpsOMColorProfileResource</a> interface pointer is to be replaced.


### -param object [in]

The <a href="https://msdn.microsoft.com/8a344300-c3fc-4225-bfa5-d5d33798a094">IXpsOMColorProfileResource</a> interface pointer that will replace current contents at the location specified by <i>index</i>.


## -returns



If the method succeeds, it returns S_OK; otherwise, it returns an <b>HRESULT</b> error code.




## -remarks



At the location specified by <i>index</i>, this method releases the <a href="https://msdn.microsoft.com/8a344300-c3fc-4225-bfa5-d5d33798a094">IXpsOMColorProfileResource</a> interface referenced by the existing pointer, then writes the pointer that is passed in <i>object</i>.

For more information about the collection methods, see  <a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>.




## -see-also




<a href="https://msdn.microsoft.com/8a344300-c3fc-4225-bfa5-d5d33798a094">IXpsOMColorProfileResource</a>



<a href="https://msdn.microsoft.com/cb9253f3-461e-47a3-820b-bb6bf5e30210">IXpsOMColorProfileResourceCollection</a>



<a href="https://msdn.microsoft.com/6ea311c0-a155-47de-ad40-62b0cbeb6e8f">Working with XPS OM Collection Interfaces</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>
 

 

