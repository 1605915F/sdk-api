---
UID: NN:xpsobjectmodel.IXpsOMGeometry
title: IXpsOMGeometry
author: windows-sdk-content
description: Describes the shape of a path or of a clipping region.
old-location: xps\ixpsomgeometry.htm
tech.root: printdocs
ms.assetid: d3f74c1e-49ef-40ee-a2f4-b6d198b57624
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IXpsOMGeometry, IXpsOMGeometry interface [XPS Documents and Packaging], IXpsOMGeometry interface [XPS Documents and Packaging],described, xps.ixpsomgeometry, xpsobjectmodel/IXpsOMGeometry
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IXpsOMGeometry
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXpsOMGeometry interface


## -description


Describes the shape of a path or of a clipping region.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IXpsOMGeometry</b> interface inherits from <a href="https://msdn.microsoft.com/2071292f-b898-4ec8-99f7-294c8d820965">IXpsOMShareable</a>. <b>IXpsOMGeometry</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IXpsOMGeometry</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/79f48f2e-884f-4afd-8f08-3285faf6c217">Clone</a>
</td>
<td align="left" width="63%">
Makes a deep copy of the interface.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c49566d6-8a37-4ad6-9b3a-52ef39b925be">GetFigures</a>
</td>
<td align="left" width="63%">
Gets a pointer to the geometry's <a href="https://msdn.microsoft.com/24ed79ff-9160-4e9b-b322-c538b30f113b">IXpsOMGeometryFigureCollection</a> interface, which  contains the collection of  figures that make up this geometry.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5ec2cfdd-f05d-4e05-b290-fad175fe1cae">GetFillRule</a>
</td>
<td align="left" width="63%">
Gets the  <a href="https://msdn.microsoft.com/353a4dc3-0c4d-46df-ae31-cc94c4116ca3">XPS_FILL_RULE</a> value that describes the fill rule to be used.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2247aa7b-28b3-459e-b565-d52a6cff7323">GetTransform</a>
</td>
<td align="left" width="63%">
Gets a pointer to the geometry's <a href="https://msdn.microsoft.com/d21457bc-9445-4ca2-ab9f-1e3f55e2e635">IXpsOMMatrixTransform</a> interface, which contains the resolved matrix transform for the geometry.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1ae895a1-7b63-460c-b066-d8e9c7cd03c2">GetTransformLocal</a>
</td>
<td align="left" width="63%">
Gets a pointer to the <a href="https://msdn.microsoft.com/d21457bc-9445-4ca2-ab9f-1e3f55e2e635">IXpsOMMatrixTransform</a> interface that contains the local, unshared matrix transform for the geometry.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/21a9a2c5-c9f2-42a4-84c4-8f702950d7ba">GetTransformLookup</a>
</td>
<td align="left" width="63%">
Gets the lookup key for the <a href="https://msdn.microsoft.com/d21457bc-9445-4ca2-ab9f-1e3f55e2e635">IXpsOMMatrixTransform</a> interface that contains the resolved matrix transform for the geometry.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/e219a505-48e0-46b0-a739-d46fb898bc58">SetFillRule</a>
</td>
<td align="left" width="63%">
Sets the  <a href="https://msdn.microsoft.com/353a4dc3-0c4d-46df-ae31-cc94c4116ca3">XPS_FILL_RULE</a> value that describes the fill rule to be used.
            

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ca4a458d-e2e5-4f8c-aac1-35f5ff91a0d9">SetTransformLocal</a>
</td>
<td align="left" width="63%">
Sets the local, unshared matrix transform.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/98623f23-eb34-4140-8179-46786ab18fb0">SetTransformLookup</a>
</td>
<td align="left" width="63%">
Sets the lookup key name of a shared matrix transform in a resource dictionary.

</td>
</tr>
</table> 


## -remarks



The code example that follows illustrates how to create an instance of  this interface.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>
IXpsOMGeometry    *newInterface;

// Note the implicit requirement that CoInitializeEx 
//  has previously been called from this thread.

hr = CoCreateInstance(
    __uuidof(XpsOMObjectFactory),
    NULL,
    CLSCTX_INPROC_SERVER,
    _uuidof(IXpsOMObjectFactory),
    reinterpret_cast&lt;LPVOID*&gt;(&amp;xpsFactory)
    );

if (SUCCEEDED(hr))
{
    hr = xpsFactory-&gt;CreateGeometry (&amp;newInterface);
    if (SUCCEEDED(hr))
    {
        // use newInterface

        newInterface-&gt;Release();
    }
    xpsFactory-&gt;Release();
}
else
{
    // evaluate HRESULT error returned in hr
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/e6933542-eb88-4936-a1d7-8380afc61557">IXpsOMObjectFactory::CreateGeometry</a>



<a href="https://msdn.microsoft.com/2071292f-b898-4ec8-99f7-294c8d820965">IXpsOMShareable</a>



<a href="https://msdn.microsoft.com/8d72ff28-6dfb-4fa8-a1b6-14b054aa7eb5">Interfaces</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>
 

 

