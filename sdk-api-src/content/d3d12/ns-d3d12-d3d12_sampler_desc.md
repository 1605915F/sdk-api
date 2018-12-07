---
UID: NS:d3d12.D3D12_SAMPLER_DESC
title: D3D12_SAMPLER_DESC
author: windows-sdk-content
description: Describes a sampler state.
old-location: direct3d12\d3d12_sampler_desc.htm
tech.root: direct3d12
ms.assetid: 96261FE1-89D4-4135-B5C4-2D788DF4FA12
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D12_SAMPLER_DESC, D3D12_SAMPLER_DESC structure, d3d12/D3D12_SAMPLER_DESC, direct3d12.d3d12_sampler_desc
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - D3D12.h
api_name:
 - D3D12_SAMPLER_DESC
product: Windows
targetos: Windows
req.typenames: D3D12_SAMPLER_DESC
req.redist: 
---

# D3D12_SAMPLER_DESC structure


## -description


Describes a sampler state.


## -struct-fields




### -field Filter

A <a href="https://msdn.microsoft.com/3755A722-34E5-415E-8760-93094D033E05">D3D12_FILTER</a>-typed value that specifies the filtering method to use when sampling a texture.
          


### -field AddressU

A <a href="https://msdn.microsoft.com/en-us/library/Dn770441(v=VS.85).aspx">D3D12_TEXTURE_ADDRESS_MODE</a>-typed value that specifies the method to use for resolving a u texture coordinate that is outside the 0 to 1 range.
          


### -field AddressV

A <a href="https://msdn.microsoft.com/en-us/library/Dn770441(v=VS.85).aspx">D3D12_TEXTURE_ADDRESS_MODE</a>-typed value that specifies the method to use for resolving a v texture coordinate that is outside the 0 to 1 range.
          


### -field AddressW

A <a href="https://msdn.microsoft.com/en-us/library/Dn770441(v=VS.85).aspx">D3D12_TEXTURE_ADDRESS_MODE</a>-typed value that specifies the method to use for resolving a w texture coordinate that is outside the 0 to 1 range.
          


### -field MipLODBias

Offset from the calculated mipmap level. For example, if the runtime calculates that a texture should be sampled at mipmap level 3 and <b>MipLODBias</b> is 2, the texture will be sampled at mipmap level 5.
          


### -field MaxAnisotropy

Clamping value used if <b>D3D12_FILTER_ANISOTROPIC</b> or <b>D3D12_FILTER_COMPARISON_ANISOTROPIC</b> is specified in <b>Filter</b>. Valid values are between 1 and 16.
          


### -field ComparisonFunc

A <a href="https://msdn.microsoft.com/en-us/library/Dn770349(v=VS.85).aspx">D3D12_COMPARISON_FUNC</a>-typed value that specifies a function that compares sampled data against existing sampled data.
          


### -field BorderColor

Border color to use if <a href="https://msdn.microsoft.com/en-us/library/Dn770441(v=VS.85).aspx">D3D12_TEXTURE_ADDRESS_MODE_BORDER</a> is specified for <b>AddressU</b>, <b>AddressV</b>, or <b>AddressW</b>. Range must be between 0.0 and 1.0 inclusive.
          


### -field MinLOD

Lower end of the mipmap range to clamp access to, where 0 is the largest and most detailed mipmap level and any level higher than that is less detailed.


### -field MaxLOD

Upper end of the mipmap range to clamp access to, where 0 is the largest and most detailed mipmap level and any level higher than that is less detailed. This value must be greater than or equal to <b>MinLOD</b>. To have no upper limit on LOD, set this member to a large value.
          


## -remarks



This structure is used by <a href="https://msdn.microsoft.com/en-us/library/Dn788671(v=VS.85).aspx">CreateSampler</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn770459(v=VS.85).aspx">Core Structures</a>
 

 

