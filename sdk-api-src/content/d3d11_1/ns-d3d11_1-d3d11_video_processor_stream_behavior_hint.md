---
UID: NS:d3d11_1.D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT
title: D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT (d3d11_1.h)
author: windows-sdk-content
description: Provides information about the input streams passed into the ID3DVideoContext1::VideoProcessorGetBehaviorHints method.
old-location: mf\d3d11_video_processor_stream_behavior_hint.htm
tech.root: medfound
ms.assetid: 0B90AB2C-3F62-49FF-A1DB-FCB07A33F482
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT, D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT structure [Media Foundation], d3d11_1/D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT, mf.d3d11_video_processor_stream_behavior_hint
ms.topic: struct
req.header: d3d11_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - d3d11_1.h
api_name:
 - D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT
product: Windows
targetos: Windows
req.typenames: D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT
req.redist: 
---

# D3D11_VIDEO_PROCESSOR_STREAM_BEHAVIOR_HINT structure


## -description


Provides information about the input streams passed into the <a href="https://msdn.microsoft.com/DDA8B3DE-A9D2-48A5-ABEE-E3F7A0EEB965">ID3DVideoContext1::VideoProcessorGetBehaviorHints</a> method.


## -struct-fields




### -field Enable

A value indicating whether this input stream should be used to compute behavior hints. Set to true if the stream should be used to compute behavior hints; otherwise, set to false.


### -field Width

The width of the input stream.


### -field Height

The height of the input stream.


### -field Format

The format of the input stream.


## -see-also




<a href="https://msdn.microsoft.com/416159A4-F50E-4027-9367-727BA81D2A21">Direct3D 11 Video Structures</a>
 

 

