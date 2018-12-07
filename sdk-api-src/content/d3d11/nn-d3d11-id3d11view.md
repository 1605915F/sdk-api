---
UID: NN:d3d11.ID3D11View
title: ID3D11View
author: windows-sdk-content
description: A view interface specifies the parts of a resource the pipeline can access during rendering.
old-location: direct3d11\id3d11view.htm
tech.root: direct3d11
ms.assetid: 060973b4-bf7d-4be2-b087-85a5b1bca905
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 0332b528-6d94-2603-1e1b-65d4d541f94f, ID3D11View, ID3D11View interface [Direct3D 11], ID3D11View interface [Direct3D 11],described, d3d11/ID3D11View, direct3d11.id3d11view
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: d3d11.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D3D11.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D11.lib
 - D3D11.dll
api_name:
 - ID3D11View
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11View interface


## -description


A view interface specifies the parts of a resource the pipeline can access during rendering.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ID3D11View</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Ff476380(v=VS.85).aspx">ID3D11DeviceChild</a>. <b>ID3D11View</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>ID3D11View</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Ff476643(v=VS.85).aspx">GetResource</a>
</td>
<td align="left" width="63%">
Get the resource that is accessed through this view.

</td>
</tr>
</table> 


## -remarks



A view interface is the base interface for all views. There are four types of views; a depth-stencil view, a render-target view, a shader-resource view, and an unordered-access view.

<ul>
<li>To create a render-target view, call <a href="https://msdn.microsoft.com/en-us/library/Ff476517(v=VS.85).aspx">ID3D11Device::CreateRenderTargetView</a>.</li>
<li>To create a depth-stencil view, call <a href="https://msdn.microsoft.com/en-us/library/Ff476507(v=VS.85).aspx">ID3D11Device::CreateDepthStencilView</a>.</li>
<li>To create a shader-resource view, call <a href="https://msdn.microsoft.com/en-us/library/Ff476519(v=VS.85).aspx">ID3D11Device::CreateShaderResourceView</a>.</li>
<li>To create an unordered-access view, call <a href="https://msdn.microsoft.com/en-us/library/Ff476523(v=VS.85).aspx">ID3D11Device::CreateUnorderedAccessView</a>.</li>
</ul>
All resources must be bound to the pipeline before they can be accessed.

<ul>
<li>To bind a render-target view or a depth-stencil view, call <a href="https://msdn.microsoft.com/en-us/library/Ff476464(v=VS.85).aspx">ID3D11DeviceContext::OMSetRenderTargets</a>.</li>
<li>To bind a shader resource, call <a href="https://msdn.microsoft.com/en-us/library/Ff476494(v=VS.85).aspx">ID3D11DeviceContext::VSSetShaderResources</a>.</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff476380(v=VS.85).aspx">ID3D11DeviceChild</a>



<a href="https://msdn.microsoft.com/en-us/library/Ff476172(v=VS.85).aspx">Resource Interfaces</a>
 

 

