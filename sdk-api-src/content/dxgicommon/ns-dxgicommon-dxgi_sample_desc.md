---
UID: NS:dxgicommon.DXGI_SAMPLE_DESC
title: DXGI_SAMPLE_DESC (dxgicommon.h)
author: windows-sdk-content
description: Describes multi-sampling parameters for a resource.
old-location: direct3ddxgi\dxgi_sample_desc.htm
tech.root: direct3ddxgi
ms.assetid: VS|directx_sdk|~\dxgi_sample_desc.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 3b41465a-e6b5-e6d1-981e-8fb841dbb6f4, DXGI_SAMPLE_DESC, DXGI_SAMPLE_DESC structure [DXGI], direct3ddxgi.dxgi_sample_desc, dxgicommon/DXGI_SAMPLE_DESC
ms.topic: struct
req.header: dxgicommon.h
req.include-header: DXGI.h
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
 - dxgicommon.h
api_name:
 - DXGI_SAMPLE_DESC
product: Windows
targetos: Windows
req.typenames: DXGI_SAMPLE_DESC
req.redist: 
---

# DXGI_SAMPLE_DESC structure


## -description


Describes multi-sampling parameters for a resource.


## -struct-fields




### -field Count

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of multisamples per pixel.


### -field Quality

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The image quality level. The higher the quality, the lower the performance. The valid range is between zero and one less than the level returned 
        by <a href="https://msdn.microsoft.com/en-us/library/Bb173537(v=VS.85).aspx">ID3D10Device::CheckMultisampleQualityLevels</a> for Direct3D 10 or <a href="https://msdn.microsoft.com/346f5dae-3ce2-4c03-ab17-1c46e18efc64">ID3D11Device::CheckMultisampleQualityLevels</a> for Direct3D 11.

For Direct3D 10.1 and Direct3D 11, you can use two special quality level values. For more information about these quality level values, see Remarks.


## -remarks



This structure is a member of the <a href="https://msdn.microsoft.com/38B302DF-5617-4195-8E4A-619D75188AD5">DXGI_SWAP_CHAIN_DESC1</a> structure.

The default sampler mode, with no anti-aliasing, has a count of 1 and a quality level of 0.

If multi-sample antialiasing is being used, all bound render targets and depth buffers must have the same sample counts and quality levels.

<table>
<tr>
<td>
Differences between Direct3D 10.0 and Direct3D 10.1 and between Direct3D 10.0 and Direct3D 11:

Direct3D 10.1 has defined two standard quality levels:  
            <b>D3D10_STANDARD_MULTISAMPLE_PATTERN</b> and <b>D3D10_CENTER_MULTISAMPLE_PATTERN</b> in the <b>D3D10_STANDARD_MULTISAMPLE_QUALITY_LEVELS</b> enumeration in D3D10_1.h.

Direct3D 11 has defined two standard quality levels:  
            <b>D3D11_STANDARD_MULTISAMPLE_PATTERN</b> and <b>D3D11_CENTER_MULTISAMPLE_PATTERN</b> in the <a href="https://msdn.microsoft.com/20c558ae-e9c3-4bab-8c11-264d626f2cff">D3D11_STANDARD_MULTISAMPLE_QUALITY_LEVELS</a> enumeration in D3D11.h.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/22e98880-bcd1-448a-9223-604fff9173fe">DXGI Structures</a>
 

 

