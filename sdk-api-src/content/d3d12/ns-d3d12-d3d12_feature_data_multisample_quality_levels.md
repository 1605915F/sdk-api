---
UID: NS:d3d12.D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS
title: D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS (d3d12.h)
author: windows-sdk-content
description: Describes the multi-sampling image quality levels for a given format and sample count.
old-location: direct3d12\d3d12_feature_data_multisample_quality_levels.htm
tech.root: direct3d12
ms.assetid: F3ECEF7C-F4A4-4134-9671-21AE488D8183
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS, D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS structure, d3d12/D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS, direct3d12.d3d12_feature_data_multisample_quality_levels
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
 - D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS
product: Windows
targetos: Windows
req.typenames: D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS
req.redist: 
---

# D3D12_FEATURE_DATA_MULTISAMPLE_QUALITY_LEVELS structure


## -description


Describes the multi-sampling image quality levels for a given format and sample count.


## -struct-fields




### -field Format

A <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a>-typed value for the format to return info about.
          


### -field SampleCount

The number of multi-samples per pixel to return info about.
          


### -field Flags

Flags to control quality levels, as a bitwise-OR'd combination of <a href="https://msdn.microsoft.com/78FBD851-879C-4C84-ACEA-58CF4ADE29A0">D3D12_MULTISAMPLE_QUALITY_LEVEL_FLAGS</a> enumeration constants.
            The resulting value specifies options for determining quality levels.
          


### -field NumQualityLevels

The number of quality levels.
          


## -remarks



See <a href="https://msdn.microsoft.com/165ECFE0-1B18-4A26-8B9C-3CE53776A349">D3D12_FEATURE</a>.
      




## -see-also




<a href="https://msdn.microsoft.com/7FE8796A-98D1-4333-8755-2A47567460B3">Core Structures</a>



<a href="https://msdn.microsoft.com/165ECFE0-1B18-4A26-8B9C-3CE53776A349">D3D12_FEATURE</a>
 

 

