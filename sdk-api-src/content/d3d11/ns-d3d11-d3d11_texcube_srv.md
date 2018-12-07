---
UID: NS:d3d11.D3D11_TEXCUBE_SRV
title: D3D11_TEXCUBE_SRV
author: windows-sdk-content
description: Specifies the subresource from a cube texture to use in a shader-resource view.
old-location: direct3d11\d3d11_texcube_srv.htm
tech.root: direct3d11
ms.assetid: ca320e06-699f-44f9-9a66-93746935b4cd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D11_TEXCUBE_SRV, D3D11_TEXCUBE_SRV structure [Direct3D 11], a217170b-8039-8202-2646-a617e73d0023, d3d11/D3D11_TEXCUBE_SRV, direct3d11.d3d11_texcube_srv
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3d11.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - D3D11.h
api_name:
 - D3D11_TEXCUBE_SRV
product: Windows
targetos: Windows
req.typenames: D3D11_TEXCUBE_SRV
req.redist: 
---

# D3D11_TEXCUBE_SRV structure


## -description


Specifies the subresource from a cube texture to use in a shader-resource view.


## -struct-fields




### -field MostDetailedMip

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

Index of the most detailed mipmap level to use; this number is between 0 and <b>MipLevels</b> (from the original TextureCube for which <a href="https://msdn.microsoft.com/en-us/library/Ff476519(v=VS.85).aspx">ID3D11Device::CreateShaderResourceView</a> creates a view) -1.


### -field MipLevels

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

The maximum number of mipmap levels for the view of the texture. See the remarks in <a href="https://msdn.microsoft.com/en-us/library/Ff476231(v=VS.85).aspx">D3D11_TEX1D_SRV</a>.

Set to -1 to indicate all the mipmap levels from <b>MostDetailedMip</b> on down to least detailed.


## -remarks



This structure is one member of a shader-resource-view description (see <a href="https://msdn.microsoft.com/en-us/library/Ff476211(v=VS.85).aspx">D3D11_SHADER_RESOURCE_VIEW_DESC</a>).




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff476173(v=VS.85).aspx">Resource Structures</a>
 

 

