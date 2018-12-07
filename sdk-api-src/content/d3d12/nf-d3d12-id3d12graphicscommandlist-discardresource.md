---
UID: NF:d3d12.ID3D12GraphicsCommandList.DiscardResource
title: ID3D12GraphicsCommandList::DiscardResource
author: windows-sdk-content
description: Discards a resource.
old-location: direct3d12\id3d12graphicscommandlist_discardresource.htm
tech.root: direct3d12
ms.assetid: 2F4DBA5B-F586-4126-8867-BEE650F6D161
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DiscardResource, DiscardResource method, DiscardResource method,ID3D12GraphicsCommandList interface, ID3D12GraphicsCommandList interface,DiscardResource method, ID3D12GraphicsCommandList.DiscardResource, ID3D12GraphicsCommandList::DiscardResource, d3d12/ID3D12GraphicsCommandList::DiscardResource, direct3d12.id3d12graphicscommandlist_discardresource
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d12.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D3d12.lib
req.dll: D3d12.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - d3d12.dll
api_name:
 - ID3D12GraphicsCommandList.DiscardResource
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12GraphicsCommandList::DiscardResource


## -description


Discards a resource.


## -parameters




### -param pResource [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn788709(v=VS.85).aspx">ID3D12Resource</a>*</b>

A pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dn788709(v=VS.85).aspx">ID3D12Resource</a> interface for the resource to discard.
            


### -param pRegion [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/Dn986726(v=VS.85).aspx">D3D12_DISCARD_REGION</a>*</b>

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/Dn986726(v=VS.85).aspx">D3D12_DISCARD_REGION</a> structure that describes details for the discard-resource operation.
            


## -returns



This method does not return a value.
          




## -remarks



The semantics of <b>DiscardResource</b> change based on the command list type.

 For <a href="https://msdn.microsoft.com/en-us/library/Dn770348(v=VS.85).aspx">D3D12_COMMAND_LIST_TYPE_DIRECT</a>, the following two rules apply:


<ul>
<li>When a resource has the <a href="https://msdn.microsoft.com/en-us/library/Dn986742(v=VS.85).aspx">D3D12_RESOURCE_FLAG_ALLOW_RENDER_TARGET</a> flag, <b>DiscardResource</b> must be called when the discarded subresource regions are in the <a href="https://msdn.microsoft.com/en-us/library/Dn986744(v=VS.85).aspx">D3D12_RESOURCE_STATE_RENDER_TARGET</a> resource barrier state.</li>
<li>When a resource has the <a href="https://msdn.microsoft.com/en-us/library/Dn986742(v=VS.85).aspx">D3D12_RESOURCE_FLAG _ALLOW_DEPTH_STENCIL</a> flag, <b>DiscardResource</b> must be called when the discarded subresource regions are in the <a href="https://msdn.microsoft.com/en-us/library/Dn986744(v=VS.85).aspx">D3D12_RESOURCE_STATE_DEPTH_WRITE</a>.
</li>
</ul>
For <a href="https://msdn.microsoft.com/en-us/library/Dn770348(v=VS.85).aspx">D3D12_COMMAND_LIST_TYPE_COMPUTE</a>, the following rule applies:


<ul>
<li>The resource must have the <a href="https://msdn.microsoft.com/en-us/library/Dn986742(v=VS.85).aspx">D3D12_RESOURCE_FLAG_ALLOW_UNORDERED_ACCESS</a> flag, and <b>DiscardResource</b> must be called when the discarded subresource regions are in the <a href="https://msdn.microsoft.com/en-us/library/Dn986744(v=VS.85).aspx">D3D12_RESOURCE_STATE_UNORDERED_ACCESS</a> resource barrier state.</li>
</ul>
<b>DiscardResource</b> is not supported on command lists with either <a href="https://msdn.microsoft.com/en-us/library/Dn770348(v=VS.85).aspx">D3D12_COMMAND_LIST_TYPE_BUNDLE</a> nor <b>D3D12_COMMAND_LIST_TYPE_COPY</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn903537(v=VS.85).aspx">ID3D12GraphicsCommandList</a>



<a href="https://msdn.microsoft.com/en-us/library/Dn899226(v=VS.85).aspx">Using Resource Barriers to Synchronize Resource States in Direct3D 12</a>
 

 

