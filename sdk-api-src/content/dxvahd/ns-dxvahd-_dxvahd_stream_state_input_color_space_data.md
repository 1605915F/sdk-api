---
UID: NS:dxvahd._DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA
title: "_DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA"
author: windows-sdk-content
description: Specifies the color space for a Microsoft DirectX Video Acceleration High Definition (DXVA-HD) input stream.
old-location: mf\dxvahd_stream_state_input_color_space_data.htm
tech.root: medfound
ms.assetid: 54b53e4d-990b-4496-aae6-039f443337ae
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA, DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA structure [Media Foundation], _DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA, dxvahd/DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA, mf.dxvahd_stream_state_input_color_space_data
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: dxvahd.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - dxvahd.h
api_name:
 - DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA
product: Windows
targetos: Windows
req.typenames: DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA
req.redist: 
---

# _DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA structure


## -description


Specifies the color space for a Microsoft DirectX Video Acceleration High Definition (DXVA-HD) input stream.


## -struct-fields




### -field Type

Specifies whether the input stream contains video or graphics. The device can optimize the processing based on the type. The default state value is 0 (video).

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0</dt>
</dl>
</td>
<td width="60%">
Video.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>1</dt>
</dl>
</td>
<td width="60%">
Graphics.

</td>
</tr>
</table>
 


### -field RGB_Range

Specifies the RGB color range. The default state value is 0 (full range).

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0</dt>
</dl>
</td>
<td width="60%">
Full range (0-255).

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>1</dt>
</dl>
</td>
<td width="60%">
Limited range (16-235).

</td>
</tr>
</table>
 


### -field YCbCr_Matrix

Specifies the YCbCr transfer matrix. The default state value is 0 (BT.601).

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0</dt>
</dl>
</td>
<td width="60%">
ITU-R BT.601.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>1</dt>
</dl>
</td>
<td width="60%">
ITU-R BT.709.

</td>
</tr>
</table>
 


### -field YCbCr_xvYCC

Specifies whether the input stream uses conventional YCbCr or extended YCbCr (xvYCC). The default state value is 0 (conventional YCbCr).

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>0</dt>
</dl>
</td>
<td width="60%">
Conventional YCbCr.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>1</dt>
</dl>
</td>
<td width="60%">
Extended YCbCr (xvYCC).

</td>
</tr>
</table>
 


### -field Reserved

 


### -field Value

 




## -remarks



The <b>RGB_Range</b> member applies to RGB input, while the <b>YCbCr_Matrix</b> and <b>YCbCr_xvYCC</b> members apply to YCbCr (YUV) input.

In some situations, the device might perform an intermediate color conversion on the input stream. If so, it uses the flags that apply to  both color spaces. For example, suppose the device converts from RGB to YCbCr. If the <b>RGB_Range</b> member is 0 and the <b>YCbCr_Matrix</b> member is 1, the device will convert from full-range RGB to BT.709 YCbCr.

If the device supports xvYCC, it returns the <b>DXVAHD_DEVICE_CAPS_xvYCC</b> capability flag in the <b>DeviceCaps</b>  member of the <a href="https://msdn.microsoft.com/340669d4-2a84-4030-83c3-a61469fdfd61">DXVAHD_VPDEVCAPS</a> structure. Otherwise, the device ignores the value of <b>YCbCr_xvYCC</b> and treats all YCbCr input as conventional YCbCr. To get the device's capabilities, call <a href="https://msdn.microsoft.com/93acad97-feee-46a5-95bf-51e560f91057">IDXVAHD_Device::GetVideoProcessorDeviceCaps</a>.


#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>HRESULT DXVAHD_SetInputColorSpace(
    IDXVAHD_VideoProcessor *pVP,
    UINT stream,
    BOOL bPlayback,     // TRUE = playback, FALSE = video processing
    UINT RGB_Range,     // 0 = 0-255, 1 = 16-235
    UINT YCbCr_Matrix,  // 0 = BT.601, 1 = BT.709
    UINT YCbCr_xvYCC    // 0 = Conventional YCbCr, 1 = xvYCC
    )
{
    DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE_DATA data =
    {
        bPlayback ? 0 : 1,
        RGB_Range ? 1 : 0,
        YCbCr_Matrix ? 1 : 0,
        YCbCr_xvYCC ? 1 : 0
    };

    HRESULT hr = pVP-&gt;SetVideoProcessStreamState(
        stream,
        DXVAHD_STREAM_STATE_INPUT_COLOR_SPACE,
        sizeof(data),
        &amp;data
        );

    return hr;
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/38ebec28-c4fc-4e72-ac87-1e41707d1908">DXVA-HD</a>



<a href="https://msdn.microsoft.com/75036101-7498-4d66-afc3-df76ae3cca39">DXVAHD_STREAM_STATE</a>



<a href="https://msdn.microsoft.com/584c087e-53f0-42d8-99ed-a0d013379363">Direct3D Video Structures</a>



<a href="https://msdn.microsoft.com/40a8444f-576e-40ff-804e-0912812f0ee6">IDXVAHD_VideoProcessor::SetVideoProcessStreamState</a>



<a href="https://msdn.microsoft.com/39fdd724-13ca-48ab-8a55-93529d1da3b4">Media Foundation Structures</a>
 

 

