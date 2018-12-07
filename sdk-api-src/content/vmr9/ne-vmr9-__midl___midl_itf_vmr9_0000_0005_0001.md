---
UID: NE:vmr9.__MIDL___MIDL_itf_vmr9_0000_0005_0001
title: "__MIDL___MIDL_itf_vmr9_0000_0005_0001"
author: windows-sdk-content
description: The VMR9MixerPrefs enumeration type contains flags that specify how the Video Mixing Render 9 filter (VMR-9) mixes the video streams. Settings include decimation, filtering, and render target preferences.
old-location: dshow\vmr9mixerprefs.htm
tech.root: DirectShow
ms.assetid: 59d3af89-248e-43cd-b6dc-e6c0a4d5f5fb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MixerPref9_ARAdjustXorY, MixerPref9_AnisotropicFiltering, MixerPref9_BiLinearFiltering, MixerPref9_DecimateMask, MixerPref9_DecimateOutput, MixerPref9_DynamicDecimateBy2, MixerPref9_DynamicMask, MixerPref9_DynamicReserved, MixerPref9_DynamicSwitchToBOB, MixerPref9_FilteringMask, MixerPref9_FilteringReserved, MixerPref9_GaussianQuadFiltering, MixerPref9_NoDecimation, MixerPref9_NonSquareMixing, MixerPref9_PointFiltering, MixerPref9_PyramidalQuadFiltering, MixerPref9_RenderTargetMask, MixerPref9_RenderTargetRGB, MixerPref9_RenderTargetReserved, MixerPref9_RenderTargetYUV, VMR9MixerPrefs, VMR9MixerPrefs , VMR9MixerPrefs enumeration [DirectShow], VMR9MixerPrefsEnumeration, __MIDL___MIDL_itf_vmr9_0000_0005_0001, dshow.vmr9mixerprefs, vmr9/MixerPref9_ARAdjustXorY, vmr9/MixerPref9_AnisotropicFiltering, vmr9/MixerPref9_BiLinearFiltering, vmr9/MixerPref9_DecimateMask, vmr9/MixerPref9_DecimateOutput, vmr9/MixerPref9_DynamicDecimateBy2, vmr9/MixerPref9_DynamicMask, vmr9/MixerPref9_DynamicReserved, vmr9/MixerPref9_DynamicSwitchToBOB, vmr9/MixerPref9_FilteringMask, vmr9/MixerPref9_FilteringReserved, vmr9/MixerPref9_GaussianQuadFiltering, vmr9/MixerPref9_NoDecimation, vmr9/MixerPref9_NonSquareMixing, vmr9/MixerPref9_PointFiltering, vmr9/MixerPref9_PyramidalQuadFiltering, vmr9/MixerPref9_RenderTargetMask, vmr9/MixerPref9_RenderTargetRGB, vmr9/MixerPref9_RenderTargetReserved, vmr9/MixerPref9_RenderTargetYUV, vmr9/VMR9MixerPrefs
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: vmr9.h
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
 - Vmr9.h
api_name:
 - VMR9MixerPrefs
product: Windows
targetos: Windows
req.typenames: VMR9MixerPrefs
req.redist: 
---

# __MIDL___MIDL_itf_vmr9_0000_0005_0001 enumeration


## -description



The <code>VMR9MixerPrefs</code> enumeration type contains flags that specify how the Video Mixing Render 9 filter (VMR-9) mixes the video streams. Settings include decimation, filtering, and render target preferences.




## -enum-fields




### -field MixerPref9_NoDecimation

No decimation. The video will be rendered onto the surface in its native size.


### -field MixerPref9_DecimateOutput

Decimate output by 2 in the x and y directions.


### -field MixerPref9_ARAdjustXorY

Adjust the horizontal or vertical size of the video streams to match the target aspect ratio. If this flag is not present, the VMR adjusts the horizontal size only. Requires Windows XP Service Pack 2. For more information, see <a href="https://msdn.microsoft.com/0ed6010b-9168-44b1-be49-0c9d5d77ce3f">Aspect Ratio Correction</a>.


### -field MixerPref9_NonSquareMixing

Do not perform aspect ratio correction on the composited stream if the input video streams have the same aspect ratio. Requires Windows XP Service Pack 2. For more information, see <a href="https://msdn.microsoft.com/8d27a921-5638-43ac-807d-e3bd7b9b2de8">Non-Square Mixing</a>.


### -field MixerPref9_DecimateMask

Bitmask to isolate the flags that control decimation. (This value is not a valid flag.)
          


### -field MixerPref9_BiLinearFiltering

Bilinear interpolation filtering. A weighted average of a 2 x 2 area of neighboring pixels is used.
          


### -field MixerPref9_PointFiltering

Point filtering. The value of the nearest is pixel is used.
          


### -field MixerPref9_AnisotropicFiltering

Anisotropic filtering.
          


### -field MixerPref9_PyramidalQuadFiltering

Four-sample tent filtering.
          


### -field MixerPref9_GaussianQuadFiltering

Four-sample Gaussian filtering.
          


### -field MixerPref9_FilteringReserved

Reserved for future use.
          


### -field MixerPref9_FilteringMask

Bitmask to isolate flags that control filtering. (This value is not a valid flag.)
          


### -field MixerPref9_RenderTargetRGB

Use an RGB render target.
          


### -field MixerPref9_RenderTargetYUV

Indicates that the target is a YUV surface. Requires Windows XP Service Pack 2. For more information, see <a href="https://msdn.microsoft.com/296b1d96-1824-4000-8bec-158925555177">YUV Mixing Mode</a>.


### -field MixerPref9_RenderTargetReserved

Reserved for future use.


### -field MixerPref9_RenderTargetMask

Bitmaks to isolate flags that control the render target. (This value is not a valid flag.)


### -field MixerPref9_DynamicSwitchToBOB

In YUV mixing mode only, this flag switches the VMR to bob deinterlacing. You can add or remove this flag while the filter graph is running; the change is applied when the VMR mixer composes the next video frame.


### -field MixerPref9_DynamicDecimateBy2

In YUV mixing mode only, this flag causes the VMR to decimate the image by a factor of 2 horizontally and vertically. You can add or remove this flag while the filter graph is running; the change will be applied when the VMR mixer composes the next video frame.


### -field MixerPref9_DynamicReserved

Reserved.


### -field MixerPref9_DynamicMask

Bitmask to isolate the MixerPref9_DynamicSwitchToBOB and MixerPref9_DynamicDecimateBy2 flags. (This value is not a valid flag.)


## -see-also




<a href="https://msdn.microsoft.com/74467006-b077-49c0-8573-f939ac3d3444">DirectShow Enumerated Types</a>



<a href="https://msdn.microsoft.com/25df0310-124a-48a5-b0fc-bea1dfd35781">IVMRMixerControl9::GetMixingPrefs</a>



<a href="https://msdn.microsoft.com/db5bf775-685c-4137-846d-fe71cddce08d">IVMRMixerControl9::SetMixingPrefs</a>
 

 

