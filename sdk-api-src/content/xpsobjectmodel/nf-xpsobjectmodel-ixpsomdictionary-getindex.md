---
UID: NF:xpsobjectmodel.IXpsOMDictionary.GetIndex
title: IXpsOMDictionary::GetIndex
author: windows-sdk-content
description: Gets the index of an IXpsOMShareable interface from the dictionary.
old-location: xps\ixpsomdictionary_getindex.htm
tech.root: printdocs
ms.assetid: dd3d8ff2-8674-4669-b7c5-6f97c957cc64
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetIndex, GetIndex method [XPS Documents and Packaging], GetIndex method [XPS Documents and Packaging],IXpsOMDictionary interface, IXpsOMDictionary interface [XPS Documents and Packaging],GetIndex method, IXpsOMDictionary.GetIndex, IXpsOMDictionary::GetIndex, xps.ixpsomdictionary_getindex, xpsobjectmodel/IXpsOMDictionary::GetIndex
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IXpsOMDictionary.GetIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMDictionary::GetIndex


## -description


Gets the index of an <a href="https://msdn.microsoft.com/2071292f-b898-4ec8-99f7-294c8d820965">IXpsOMShareable</a> interface from the dictionary.


## -parameters




### -param entry [in]

The <a href="https://msdn.microsoft.com/2071292f-b898-4ec8-99f7-294c8d820965">IXpsOMShareable</a> interface pointer to be found in the dictionary.


### -param index [out, retval]

The zero-based index of <i>entry</i> in the dictionary.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the table that follows. For information about  XPS document API return values that are not listed in this table, see <a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>.

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
<dt><b>E_INVALIDARG
</b></dt>
</dl>
</td>
<td width="60%">
The object referenced by <i>entry</i> is not in the dictionary.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/f887e3d3-973c-4267-a785-6bc190c13082">IXpsOMDictionary</a>



<a href="https://msdn.microsoft.com/2071292f-b898-4ec8-99f7-294c8d820965">IXpsOMShareable</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>
 

 

