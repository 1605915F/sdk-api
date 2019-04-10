---
UID: NF:xpsobjectmodel.IXpsOMTileBrush.GetTransformLookup
title: IXpsOMTileBrush::GetTransformLookup (xpsobjectmodel.h)
author: windows-sdk-content
description: Gets the lookup key that identifies the IXpsOMMatrixTransform interface in a resource dictionary that contains the resolved matrix transform for the brush.
old-location: xps\ixpsomtilebrush_gettransformlookup.htm
tech.root: printdocs
ms.assetid: bebed09b-7af7-4da1-aaa3-e8e2a45f2717
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetTransformLookup, GetTransformLookup method [XPS Documents and Packaging], GetTransformLookup method [XPS Documents and Packaging],IXpsOMTileBrush interface, IXpsOMTileBrush interface [XPS Documents and Packaging],GetTransformLookup method, IXpsOMTileBrush.GetTransformLookup, IXpsOMTileBrush::GetTransformLookup, xps.ixpsomtilebrush_gettransformlookup, xpsobjectmodel/IXpsOMTileBrush::GetTransformLookup
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
 - IXpsOMTileBrush.GetTransformLookup
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMTileBrush::GetTransformLookup


## -description


Gets the lookup key that identifies the <a href="https://msdn.microsoft.com/d21457bc-9445-4ca2-ab9f-1e3f55e2e635">IXpsOMMatrixTransform</a> interface in a resource dictionary that contains the resolved matrix transform for the brush.


## -parameters




### -param key [out, retval]

The lookup key that identifies the <a href="https://msdn.microsoft.com/d21457bc-9445-4ca2-ab9f-1e3f55e2e635">IXpsOMMatrixTransform</a> interface in a resource dictionary that contains the resolved matrix transform for the brush. If a matrix transform lookup key has not been set or if a local matrix transform has  been set, a <b>NULL</b> pointer is returned.

<table>
<tr>
<th>Most recent method called</th>
<th>Object that is returned  in <i>key</i></th>
</tr>
<tr>
<td>

<a href="https://msdn.microsoft.com/a0a0f0e9-d8b5-4b42-804b-66780f56b09a">SetTransformLocal</a>


</td>
<td>
<b>NULL</b> pointer.

</td>
</tr>
<tr>
<td>

<a href="https://msdn.microsoft.com/b2d9519a-9e22-44ba-839d-e1ba33aacc26">SetTransformLookup</a>


</td>
<td>
The lookup key  set by <a href="https://msdn.microsoft.com/b2d9519a-9e22-44ba-839d-e1ba33aacc26">SetTransformLookup</a>.

</td>
</tr>
<tr>
<td>
Neither <a href="https://msdn.microsoft.com/a0a0f0e9-d8b5-4b42-804b-66780f56b09a">SetTransformLocal</a> nor <a href="https://msdn.microsoft.com/b2d9519a-9e22-44ba-839d-e1ba33aacc26">SetTransformLookup</a> has been called yet.

</td>
<td>
<b>NULL</b> pointer.

</td>
</tr>
</table>
 


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
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<i>key</i> is <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



The transform determines how the output area is transformed before the brush image is rendered in the path, stroke, or glyph that is using the tile brush.

This method allocates the memory used by the string that is returned in <i>key</i>.  If <i>key</i> is not <b>NULL</b>, use the <a href="https://msdn.microsoft.com/en-us/library/ms680722(v=VS.85).aspx">CoTaskMemFree</a> function  to free the memory.




## -see-also




<a href="https://msdn.microsoft.com/d21457bc-9445-4ca2-ab9f-1e3f55e2e635">IXpsOMMatrixTransform</a>



<a href="https://msdn.microsoft.com/fc9e1925-0dbc-447b-9acc-e7f719df62d1">IXpsOMTileBrush</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>



<a href="https://msdn.microsoft.com/9e6db1e3-7151-4538-8607-b7185ebc0110">XPS Document Errors</a>
 

 

