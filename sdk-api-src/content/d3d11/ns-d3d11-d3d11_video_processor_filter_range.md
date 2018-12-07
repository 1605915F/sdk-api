---
UID: NS:d3d11.D3D11_VIDEO_PROCESSOR_FILTER_RANGE
title: D3D11_VIDEO_PROCESSOR_FILTER_RANGE
author: windows-sdk-content
description: Defines the range of supported values for an image filter.
old-location: mf\d3d11_video_processor_filter_range.htm
tech.root: medfound
ms.assetid: 22B11763-717A-49D7-8F5B-2FD21C13F11E
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D11_VIDEO_PROCESSOR_FILTER_RANGE, D3D11_VIDEO_PROCESSOR_FILTER_RANGE structure [Media Foundation], d3d11/D3D11_VIDEO_PROCESSOR_FILTER_RANGE, mf.d3d11_video_processor_filter_range
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3d11.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
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
 - d3d11.h
api_name:
 - D3D11_VIDEO_PROCESSOR_FILTER_RANGE
product: Windows
targetos: Windows
req.typenames: D3D11_VIDEO_PROCESSOR_FILTER_RANGE
req.redist: 
---

# D3D11_VIDEO_PROCESSOR_FILTER_RANGE structure


## -description


Defines the range of supported values for an image filter.




## -struct-fields




### -field Minimum

The minimum value of the filter.




### -field Maximum

The maximum value of the filter.




### -field Default

The default value of the filter.




### -field Multiplier

A multiplier. Use the following formula to translate the filter setting into the actual filter value: <i>Actual Value</i> = <i>Set Value</i> × <i>Multiplier</i>.


## -remarks



The multiplier enables the filter range to have a fractional step value.

For example, a hue filter might have an actual range of [–180.0 ... +180.0] with a step size of 0.25. The device would report the following range and multiplier:

<ul>
<li>Minimum: –720</li>
<li>Maximum: +720</li>
<li>Multiplier: 0.25</li>
</ul>
In this case,  a filter value of 2 would be interpreted by the device as 0.50 (or 2 × 0.25).

The device should use  a multiplier that can be represented exactly as a base-2 fraction.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh447680(v=VS.85).aspx">Direct3D 11 Video Structures</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh447805(v=VS.85).aspx">ID3D11VideoProcessorEnumerator::GetVideoProcessorFilterRange</a>
 

 

