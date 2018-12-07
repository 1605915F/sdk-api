---
UID: NS:d3d11_2.D3D11_SUBRESOURCE_TILING
title: D3D11_SUBRESOURCE_TILING
author: windows-sdk-content
description: Describes a tiled subresource volume.
old-location: direct3d11\d3d11_subresource_tiling.htm
tech.root: direct3d11
ms.assetid: 679E4AD1-3AC8-4055-9D38-37776E2D17BE
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D11_SUBRESOURCE_TILING, D3D11_SUBRESOURCE_TILING structure [Direct3D 11], d3d11_2/D3D11_SUBRESOURCE_TILING, direct3d11.d3d11_subresource_tiling
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3d11_2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
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
 - HeaderDef
api_location:
 - D3D11_2.h
api_name:
 - D3D11_SUBRESOURCE_TILING
product: Windows
targetos: Windows
req.typenames: D3D11_SUBRESOURCE_TILING
req.redist: 
---

# D3D11_SUBRESOURCE_TILING structure


## -description


Describes a tiled subresource volume.


## -struct-fields




### -field WidthInTiles

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

The width in tiles of the subresource.


### -field HeightInTiles

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT16</a></b>

The height in tiles of the subresource.


### -field DepthInTiles

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT16</a></b>

The depth in tiles of the subresource.


### -field StartTileIndexInOverallResource

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

The index of the tile in the overall tiled subresource to start with. 


<a href="https://msdn.microsoft.com/en-us/library/Dn280497(v=VS.85).aspx">GetResourceTiling</a> sets <b>StartTileIndexInOverallResource</b> to <b>D3D11_PACKED_TILE</b> (0xffffffff) to indicate that the whole 
<b>D3D11_SUBRESOURCE_TILING</b> structure is meaningless, and the info to which the <i>pPackedMipDesc</i> parameter of <b>GetResourceTiling</b> points applies. For packed tiles, the description of the packed mipmaps comes from a <a href="https://msdn.microsoft.com/en-us/library/Dn280418(v=VS.85).aspx">D3D11_PACKED_MIP_DESC</a> structure instead.



## -remarks



Each packed mipmap is individually reported as 0 for <b>WidthInTiles</b>, <b>HeightInTiles</b> and <b>DepthInTiles</b>.


The total number of tiles in subresources is <b>WidthInTiles</b>*<b>HeightInTiles</b>*<b>DepthInTiles</b>. 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff476173(v=VS.85).aspx">Resource Structures</a>
 

 

