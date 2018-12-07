---
UID: NS:d3d11.D3D11_FEATURE_DATA_FORMAT_SUPPORT
title: D3D11_FEATURE_DATA_FORMAT_SUPPORT
author: windows-sdk-content
description: Describes which resources are supported by the current graphics driver for a given format.
old-location: direct3d11\d3d11_feature_data_format_support.htm
tech.root: direct3d11
ms.assetid: 153e246e-9e2f-4557-94c4-a9f1a3b926bd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D11_FEATURE_DATA_FORMAT_SUPPORT, D3D11_FEATURE_DATA_FORMAT_SUPPORT structure [Direct3D 11], a30c19a0-2294-7e25-009e-e49d1560486d, d3d11/D3D11_FEATURE_DATA_FORMAT_SUPPORT, direct3d11.d3d11_feature_data_format_support
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
 - D3D11_FEATURE_DATA_FORMAT_SUPPORT
product: Windows
targetos: Windows
req.typenames: D3D11_FEATURE_DATA_FORMAT_SUPPORT
req.redist: 
---

# D3D11_FEATURE_DATA_FORMAT_SUPPORT structure


## -description


Describes which resources are supported by the current graphics driver for a given format.


## -struct-fields




### -field InFormat

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a> to return information on.


### -field OutFormatSupport

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

Combination of <a href="https://msdn.microsoft.com/en-us/library/Ff476134(v=VS.85).aspx">D3D11_FORMAT_SUPPORT</a> flags indicating which resources are supported.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Ff476155(v=VS.85).aspx">Core Structures</a>
 

 

