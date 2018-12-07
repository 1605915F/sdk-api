---
UID: NN:d3d11_1.ID3D11RasterizerState1
title: ID3D11RasterizerState1
author: windows-sdk-content
description: The rasterizer-state interface holds a description for rasterizer state that you can bind to the rasterizer stage. This rasterizer-state interface supports forced sample count.
old-location: direct3d11\id3d11rasterizerstate1.htm
tech.root: direct3d11
ms.assetid: 771BA97B-1DC4-46DD-AAB6-DFC1100F844D
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3D11RasterizerState1, ID3D11RasterizerState1 interface [Direct3D 11], ID3D11RasterizerState1 interface [Direct3D 11],described, d3d11_1/ID3D11RasterizerState1, direct3d11.id3d11rasterizerstate1
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: d3d11_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - ID3D11RasterizerState1
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11RasterizerState1 interface


## -description


The rasterizer-state interface holds a description for rasterizer state that you can bind to the <a href="https://msdn.microsoft.com/en-us/library/Bb205125(v=VS.85).aspx">rasterizer stage</a>. This rasterizer-state interface supports forced sample count.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ID3D11RasterizerState1</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Ff476580(v=VS.85).aspx">ID3D11RasterizerState</a>. <b>ID3D11RasterizerState1</b> also has these types of members:
<ul>
<li><a href="https://msdn.microsoft.com/en-us/library/ms684591(v=VS.85).aspx">Methods</a></li>
</ul>

## -members

The <b>ID3D11RasterizerState1</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh446830(v=VS.85).aspx">GetDesc1</a>
</td>
<td align="left" width="63%">
Gets the description for rasterizer state that you used to create the rasterizer-state object.

</td>
</tr>
</table> 


## -remarks



To create a rasterizer-state object, call <a href="https://msdn.microsoft.com/en-us/library/Hh404586(v=VS.85).aspx">ID3D11Device1::CreateRasterizerState1</a>. To bind the rasterizer-state object to the <a href="https://msdn.microsoft.com/en-us/library/Bb205125(v=VS.85).aspx">rasterizer stage</a>, call <a href="https://msdn.microsoft.com/en-us/library/Ff476479(v=VS.85).aspx">ID3D11DeviceContext::RSSetState</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff476154(v=VS.85).aspx">Core Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/Ff476580(v=VS.85).aspx">ID3D11RasterizerState</a>
 

 

