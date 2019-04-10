---
UID: NE:d3d11.D3D11_RTV_DIMENSION
title: D3D11_RTV_DIMENSION (d3d11.h)
author: windows-sdk-content
description: These flags identify the type of resource that will be viewed as a render target.
old-location: direct3d11\d3d11_rtv_dimension.htm
tech.root: direct3d11
ms.assetid: 42cbd3ec-fa8a-48ea-be88-bbe46db13566
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 3ae03219-f0f0-843c-5eb9-caae0782e153, D3D11_RTV_DIMENSION, D3D11_RTV_DIMENSION enumeration [Direct3D 11], D3D11_RTV_DIMENSION_BUFFER, D3D11_RTV_DIMENSION_TEXTURE1D, D3D11_RTV_DIMENSION_TEXTURE1DARRAY, D3D11_RTV_DIMENSION_TEXTURE2D, D3D11_RTV_DIMENSION_TEXTURE2DARRAY, D3D11_RTV_DIMENSION_TEXTURE2DMS, D3D11_RTV_DIMENSION_TEXTURE2DMSARRAY, D3D11_RTV_DIMENSION_TEXTURE3D, D3D11_RTV_DIMENSION_UNKNOWN, d3d11/D3D11_RTV_DIMENSION, d3d11/D3D11_RTV_DIMENSION_BUFFER, d3d11/D3D11_RTV_DIMENSION_TEXTURE1D, d3d11/D3D11_RTV_DIMENSION_TEXTURE1DARRAY, d3d11/D3D11_RTV_DIMENSION_TEXTURE2D, d3d11/D3D11_RTV_DIMENSION_TEXTURE2DARRAY, d3d11/D3D11_RTV_DIMENSION_TEXTURE2DMS, d3d11/D3D11_RTV_DIMENSION_TEXTURE2DMSARRAY, d3d11/D3D11_RTV_DIMENSION_TEXTURE3D, d3d11/D3D11_RTV_DIMENSION_UNKNOWN, direct3d11.d3d11_rtv_dimension
ms.topic: enum
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
 - D3D11_RTV_DIMENSION
product: Windows
targetos: Windows
req.typenames: D3D11_RTV_DIMENSION
req.redist: 
---

# D3D11_RTV_DIMENSION enumeration


## -description


These flags identify the type of resource that will be viewed as a render target.


## -enum-fields




### -field D3D11_RTV_DIMENSION_UNKNOWN

Do not use this value, as it will cause <a href="https://msdn.microsoft.com/e757c959-f0ac-44c3-8226-b9f0b1c2a031">ID3D11Device::CreateRenderTargetView</a> to fail.


### -field D3D11_RTV_DIMENSION_BUFFER

The resource will be accessed as a buffer.


### -field D3D11_RTV_DIMENSION_TEXTURE1D

The resource will be accessed as a 1D texture.


### -field D3D11_RTV_DIMENSION_TEXTURE1DARRAY

The resource will be accessed as an array of 1D textures.


### -field D3D11_RTV_DIMENSION_TEXTURE2D

The resource will be accessed as a 2D texture.


### -field D3D11_RTV_DIMENSION_TEXTURE2DARRAY

The resource will be accessed as an array of 2D textures.


### -field D3D11_RTV_DIMENSION_TEXTURE2DMS

The resource will be accessed as a 2D texture with multisampling.


### -field D3D11_RTV_DIMENSION_TEXTURE2DMSARRAY

The resource will be accessed as an array of 2D textures with multisampling.


### -field D3D11_RTV_DIMENSION_TEXTURE3D

The resource will be accessed as a 3D texture.


## -remarks



This enumeration is used in <a href="https://msdn.microsoft.com/b154ac98-49ed-4d00-8cb6-5e57680e125c">D3D11_RENDER_TARGET_VIEW_DESC</a> to create a render-target view.




## -see-also




<a href="https://msdn.microsoft.com/b547819b-7006-40b5-84a4-adf198048051">Resource Enumerations</a>
 

 

