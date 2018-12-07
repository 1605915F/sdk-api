---
UID: NN:wmdxva.IWMCodecAMVideoAccelerator
title: IWMCodecAMVideoAccelerator
author: windows-sdk-content
description: This interface is exposed by the Windows Media Decoder DMO and is called by a media player source filter to set up the various connections required to enable DirectX&#174; video acceleration (VA) for decoding of Windows Media-based video content.
old-location: wmformat\iwmcodecamvideoaccelerator.htm
tech.root: wmformat
ms.assetid: 48cfc4d1-4b79-47a5-9cc9-a1f19d2c0123
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMCodecAMVideoAccelerator, IWMCodecAMVideoAccelerator interface [windows Media Format], IWMCodecAMVideoAccelerator interface [windows Media Format],described, IWMCodecAMVideoAcceleratorInterface, wmdxva/IWMCodecAMVideoAccelerator, wmformat.iwmcodecamvideoaccelerator
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: wmdxva.h
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
 - COM
api_location:
 - wmdxva.h
api_name:
 - IWMCodecAMVideoAccelerator
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMCodecAMVideoAccelerator interface


## -description



This interface is exposed by the Windows Media Decoder <a href="https://msdn.microsoft.com/en-us/library/Dd757828(v=VS.85).aspx">DMO</a> and is called by a media player source filter to set up the various connections required to enable DirectX® video acceleration (VA) for decoding of Windows Media-based video content. A player obtains this interface by calling the <a href="https://msdn.microsoft.com/e38c02bb-335c-4f93-9e98-1a9dc65a37c5">IWMReaderAccelerator::GetCodecInterface</a> method, which is exposed on the reader object.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMCodecAMVideoAccelerator</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMCodecAMVideoAccelerator</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMCodecAMVideoAccelerator</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/547c43ed-7e04-4323-9e10-019ecfdbb641">NegotiateConnection</a>
</td>
<td align="left" width="63%">
Called by the output pin on the player's source filter during the connection process when it has been given a DirectX VA media type.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6ffaa2dc-65d6-4ba0-9688-8b59fe593ecd">SetAcceleratorInterface</a>
</td>
<td align="left" width="63%">
Called by the output pin on the player's source filter to pass the VMR's <b>IAMVideoAccelerator</b> interface to the decoder DMO.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/3be015c4-a641-44b9-9be8-a76b5dd4f998">SetPlayerNotify</a>
</td>
<td align="left" width="63%">
Called by the output pin on the source filter to provide the decoder DMO with the source filter's <b>IWMPlayerTimestampHook</b> interface to enable the filter to update the time stamps on the samples before they are delivered to the renderer.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/5cb2f564-88e3-4b60-bde3-6ccf69c97c48">Enabling DirectX Video Acceleration</a>



<a href="https://msdn.microsoft.com/c61a0739-09f2-497f-a2cd-d3f2472738e3">Interfaces</a>



<a href="https://msdn.microsoft.com/b5edbf8b-820f-4e09-a482-8efc2283360e">Reader Object</a>
 

 

