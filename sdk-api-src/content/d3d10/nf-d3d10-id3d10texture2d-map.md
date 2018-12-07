---
UID: NF:d3d10.ID3D10Texture2D.Map
title: ID3D10Texture2D::Map
author: windows-sdk-content
description: Get a pointer to the data contained in a subresource, and deny GPU access to that subresource.
old-location: direct3d10\id3d10texture2d_map.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10texture2d_map.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 2f53ee75-643c-3909-1e4f-aa32b40994c3, ID3D10Texture2D interface [Direct3D 10],Map method, ID3D10Texture2D.Map, ID3D10Texture2D::Map, Map, Map method [Direct3D 10], Map method [Direct3D 10],ID3D10Texture2D interface, d3d10/ID3D10Texture2D::Map, direct3d10.id3d10texture2d_map
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d10.h
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
req.lib: D3D10.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D10.lib
 - D3D10.dll
api_name:
 - ID3D10Texture2D.Map
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10Texture2D::Map


## -description


Get a pointer to the data contained in a subresource, and deny GPU access to that subresource.


## -parameters




### -param Subresource [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

Index number of the subresource. See <a href="https://msdn.microsoft.com/en-us/library/Bb694525(v=VS.85).aspx">D3D10CalcSubresource</a> for more details.


### -param MapType [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205318(v=VS.85).aspx">D3D10_MAP</a></b>

Integer that specifies the CPU's read and write permissions for a resource. For possible values, see <a href="https://msdn.microsoft.com/en-us/library/Bb205318(v=VS.85).aspx">D3D10_MAP</a>.


### -param MapFlags [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb205321(v=VS.85).aspx">Flag</a> that specifies what the CPU should do when the GPU is busy. This flag is optional.


### -param pMappedTex2D [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205319(v=VS.85).aspx">D3D10_MAPPED_TEXTURE2D</a>*</b>

Pointer to a structure (<a href="https://msdn.microsoft.com/en-us/library/Bb205319(v=VS.85).aspx">D3D10_MAPPED_TEXTURE2D</a>) that is filled in by the function and contains a pointer to the resource data.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this function succeeds, it returns S_OK.

All of the Map methods have identical return values and operating restrictions. These are listed in the remarks section of <a href="https://msdn.microsoft.com/en-us/library/Bb173865(v=VS.85).aspx">ID3D10Texture1D::Map</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173867(v=VS.85).aspx">ID3D10Texture2D Interface</a>
 

 

