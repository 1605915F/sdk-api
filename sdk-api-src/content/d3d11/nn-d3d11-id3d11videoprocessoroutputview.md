---
UID: NN:d3d11.ID3D11VideoProcessorOutputView
title: ID3D11VideoProcessorOutputView (d3d11.h)
author: windows-sdk-content
description: Identifies the output surfaces that can be accessed during video processing.
old-location: mf\id3d11videoprocessoroutputview.htm
tech.root: medfound
ms.assetid: D07829ED-2C1E-4150-A0A1-5CD95F30209F
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ID3D11VideoProcessorOutputView, ID3D11VideoProcessorOutputView interface [Media Foundation], ID3D11VideoProcessorOutputView interface [Media Foundation],described, d3d11/ID3D11VideoProcessorOutputView, mf.id3d11videoprocessoroutputview
ms.topic: interface
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
 - ID3D11VideoProcessorOutputView
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11VideoProcessorOutputView interface


## -description


Identifies the output surfaces that can be accessed during video processing.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ID3D11VideoProcessorOutputView</b> interface inherits from <a href="https://msdn.microsoft.com/060973b4-bf7d-4be2-b087-85a5b1bca905">ID3D11View</a>. <b>ID3D11VideoProcessorOutputView</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ID3D11VideoProcessorOutputView</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/8FDC547A-64B9-415C-865C-31BF8FA1A711">GetDesc</a>
</td>
<td align="left" width="63%">
Gets the properties of the video processor output view.

</td>
</tr>
</table> 


## -remarks



To get a pointer to this interface, call <a href="https://msdn.microsoft.com/EC7AFE44-877C-4FB0-9E61-FCD504A334D3">ID3D11VideoDevice::CreateVideoProcessorOutputView</a>.




## -see-also




<a href="https://msdn.microsoft.com/2AE97FFE-0FA4-4CC0-8433-7BA46BCACE30">Direct3D 11 Video Interfaces</a>



<a href="https://msdn.microsoft.com/060973b4-bf7d-4be2-b087-85a5b1bca905">ID3D11View</a>
 

 

