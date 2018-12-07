---
UID: NF:d3d12.ID3D12GraphicsCommandList.IASetVertexBuffers
title: ID3D12GraphicsCommandList::IASetVertexBuffers
author: windows-sdk-content
description: Sets a CPU descriptor handle for the vertex buffers.
old-location: direct3d12\id3d12graphicscommandlist_iasetvertexbuffers.htm
tech.root: direct3d12
ms.assetid: AADD6CEF-376D-43AB-86E6-37B5D7DD0B25
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IASetVertexBuffers, IASetVertexBuffers method, IASetVertexBuffers method,ID3D12GraphicsCommandList interface, ID3D12GraphicsCommandList interface,IASetVertexBuffers method, ID3D12GraphicsCommandList.IASetVertexBuffers, ID3D12GraphicsCommandList::IASetVertexBuffers, d3d12/ID3D12GraphicsCommandList::IASetVertexBuffers, direct3d12.id3d12graphicscommandlist_iasetvertexbuffers
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
 - ID3D12GraphicsCommandList.IASetVertexBuffers
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12GraphicsCommandList::IASetVertexBuffers


## -description


Sets a CPU descriptor handle for the vertex buffers.


## -parameters




### -param StartSlot [in]

Type: <b>UINT</b>

Index into the device's zero-based array to begin setting vertex buffers.
          


### -param NumViews [in]

Type: <b>UINT</b>

The number of views in the <i>pViews</i> array.
          


### -param pViews [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/Dn903819(v=VS.85).aspx">D3D12_VERTEX_BUFFER_VIEW</a>*</b>

Specifies the vertex buffer views in an array of <a href="https://msdn.microsoft.com/en-us/library/Dn903819(v=VS.85).aspx">D3D12_VERTEX_BUFFER_VIEW</a> structures.
          


## -returns



This method does not return a value.
          




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn986882(v=VS.85).aspx">IASetIndexBuffer</a>



<a href="https://msdn.microsoft.com/en-us/library/Dn903537(v=VS.85).aspx">ID3D12GraphicsCommandList</a>
 

 

