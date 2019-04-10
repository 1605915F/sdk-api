---
UID: NE:d3d11.D3D11_VIDEO_PROCESSOR_FEATURE_CAPS
title: D3D11_VIDEO_PROCESSOR_FEATURE_CAPS (d3d11.h)
author: windows-sdk-content
description: Defines features that a Microsoft Direct3D 11 video processor can support.
old-location: mf\d3d11_video_processor_feature_caps.htm
tech.root: medfound
ms.assetid: A40E33D4-E8F3-4348-9135-DD56BABBFA85
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: D3D11_VIDEO_PROCESSOR_FEATURE_CAPS, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS enumeration [Media Foundation], D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_FILL, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_PALETTE, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_STREAM, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_CONSTRICTION, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_LEGACY, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_LUMA_KEY, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_PIXEL_ASPECT_RATIO, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ROTATION, D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_STEREO, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_FILL, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_PALETTE, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_STREAM, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_CONSTRICTION, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_LEGACY, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_LUMA_KEY, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_PIXEL_ASPECT_RATIO, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ROTATION, d3d11/D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_STEREO, mf.d3d11_video_processor_feature_caps
ms.topic: enum
req.header: d3d11.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - D3D11_VIDEO_PROCESSOR_FEATURE_CAPS
product: Windows
targetos: Windows
req.typenames: D3D11_VIDEO_PROCESSOR_FEATURE_CAPS
req.redist: 
---

# D3D11_VIDEO_PROCESSOR_FEATURE_CAPS enumeration


## -description


Defines features that a Microsoft Direct3D 11 video processor can support.




## -enum-fields




### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_FILL

The video processor can set alpha values on the output pixels. For more information, see <a href="https://msdn.microsoft.com/898604FA-B857-4D84-AA0D-3BC517F75A36">ID3D11VideoContext::VideoProcessorSetOutputAlphaFillMode</a>.


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_CONSTRICTION

The video processor can downsample the video output. For more information, see <a href="https://msdn.microsoft.com/EA61A4B8-0853-4F17-B634-70A896DCF5F7">ID3D11VideoContext::VideoProcessorSetOutputConstriction</a>.


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_LUMA_KEY

The video processor can perform luma keying. For more information, see <a href="https://msdn.microsoft.com/DAFDAF7C-BBE2-41AA-9E44-C1BD28CE03FE">ID3D11VideoContext::VideoProcessorSetStreamLumaKey</a>.


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_PALETTE

The video processor can apply alpha values from color palette entries. 


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_LEGACY

The driver does not support full video processing capabilities. If this capability flag is set, the video processor has the following limitations:

<ul>
<li>A maximum of two streams are supported:<ul>
<li>The first stream must be either NV12 or YUY2.</li>
<li>The second stream must be AYUV, AI44, or IA44.</li>
</ul>
</li>
<li>Image adjustment (proc amp) controls are applied to the entire video processing blit, rather than per stream.</li>
<li>Support for per-stream planar alpha is not reliable. (Per-pixel alpha is supported, however.)</li>
</ul>

### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_STEREO

The video processor can support 3D stereo video. For more information, see <a href="https://msdn.microsoft.com/FAAE902A-622E-42D2-B332-CD4126A4182E">ID3D11VideoContext::VideoProcessorSetStreamStereoFormat</a>.

All drivers setting this caps must support the following stereo formats: <a href="https://msdn.microsoft.com/77832DF2-821E-465C-80B6-46DDB2433791">D3D11_VIDEO_PROCESSOR_STEREO_FORMAT_HORIZONTAL</a>, <b>D3D11_VIDEO_PROCESSOR_STEREO_FORMAT_VERTICAL</b>, and <b>D3D11_VIDEO_PROCESSOR_STEREO_FORMAT_SEPARATE</b>.


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ROTATION

The driver can rotate the input data either 90, 180, or 270 degrees clockwise as part of the video processing operation.


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_ALPHA_STREAM

The driver supports the <a href="https://msdn.microsoft.com/DA869E3F-25BB-4794-B7AE-A3C2DA968800">VideoProcessorSetStreamAlpha</a> call.


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_PIXEL_ASPECT_RATIO

The driver supports the <a href="https://msdn.microsoft.com/4205F6F0-4AF3-42B1-8636-64FCFC865856">VideoProcessorSetStreamPixelAspectRatio</a> call.


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_MIRROR


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_SHADER_USAGE


### -field D3D11_VIDEO_PROCESSOR_FEATURE_CAPS_METADATA_HDR10




## -see-also




<a href="https://msdn.microsoft.com/EF79BE15-B92E-45C1-BC42-E89E06197C20">D3D11_VIDEO_PROCESSOR_CAPS</a>



<a href="https://msdn.microsoft.com/40061AD1-BCD9-4170-A442-34B4C792BB55">Direct3D 11 Video Enumerations</a>
 

 

