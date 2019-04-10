---
UID: NF:d3d11.ID3D11VideoContext.VideoProcessorGetStreamOutputRate
title: ID3D11VideoContext::VideoProcessorGetStreamOutputRate (d3d11.h)
author: windows-sdk-content
description: Gets the rate at which the video processor produces output frames for an input stream.
old-location: mf\id3d11videocontext_videoprocessorgetstreamoutputrate.htm
tech.root: medfound
ms.assetid: 69AC0713-FE92-4D89-857A-A0037D51B597
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FALSE, ID3D11VideoContext interface [Media Foundation],VideoProcessorGetStreamOutputRate method, ID3D11VideoContext.VideoProcessorGetStreamOutputRate, ID3D11VideoContext::VideoProcessorGetStreamOutputRate, TRUE, VideoProcessorGetStreamOutputRate, VideoProcessorGetStreamOutputRate method [Media Foundation], VideoProcessorGetStreamOutputRate method [Media Foundation],ID3D11VideoContext interface, d3d11/ID3D11VideoContext::VideoProcessorGetStreamOutputRate, mf.id3d11videocontext_videoprocessorgetstreamoutputrate
ms.topic: method
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
 - COM
api_location:
 - d3d11.h
api_name:
 - ID3D11VideoContext.VideoProcessorGetStreamOutputRate
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11VideoContext::VideoProcessorGetStreamOutputRate


## -description


Gets the rate at which the video processor produces output frames for an input stream.




## -parameters




### -param pVideoProcessor [in]

A pointer to the <a href="https://msdn.microsoft.com/AF6F6781-A7F9-4196-8E91-FDFDD1924E24">ID3D11VideoProcessor</a> interface. To get this pointer, call <a href="https://msdn.microsoft.com/5A5FB7F9-F299-4E67-AFAD-E7056CBAEE76">ID3D11VideoDevice::CreateVideoProcessor</a>.


### -param StreamIndex [in]

The zero-based index of the input stream. To get the maximum number of streams, call <a href="https://msdn.microsoft.com/BE213FFE-FB1D-4BDC-A1AA-2EA487DF8D4A">ID3D11VideoProcessorEnumerator::GetVideoProcessorCaps</a> and check the <b>MaxStreamStates</b> structure member.


### -param pOutputRate [out]

Receives a <a href="https://msdn.microsoft.com/C950E5B5-E50C-4750-83F3-38296EF2009F">D3D11_VIDEO_PROCESSOR_OUTPUT_RATE</a> value that specifies the output rate.


### -param pRepeatFrame [out]

Receives a Boolean value that specifies how the driver performs frame-rate conversion, if required.



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="TRUE"></a><a id="true"></a><dl>
<dt><b>TRUE</b></dt>
</dl>
</td>
<td width="60%">
Repeat frames.

</td>
</tr>
<tr>
<td width="40%"><a id="FALSE"></a><a id="false"></a><dl>
<dt><b>FALSE</b></dt>
</dl>
</td>
<td width="60%">
Interpolate frames.

</td>
</tr>
</table>
 


### -param pCustomRate [out]

A pointer to a <a href="https://msdn.microsoft.com/en-us/library/Bb173069(v=VS.85).aspx">DXGI_RATIONAL</a> structure. If the output rate is <b>D3D11_VIDEO_PROCESSOR_OUTPUT_RATE_CUSTOM</b>, the method fills in this structure with the exact output rate. Otherwise, this parameter is ignored.




## -returns



This method does not return a value.




## -see-also




<a href="https://msdn.microsoft.com/6EF09C31-56C7-46B5-87AE-B1FE43EC66FC">ID3D11VideoContext</a>
 

 

