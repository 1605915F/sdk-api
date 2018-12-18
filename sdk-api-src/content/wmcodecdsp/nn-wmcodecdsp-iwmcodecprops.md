---
UID: NN:wmcodecdsp.IWMCodecProps
title: IWMCodecProps
author: windows-sdk-content
description: Provides methods that retrieve format-specific codec properties.
old-location: mf\iwmcodecpropsinterface.htm
tech.root: medfound
ms.assetid: b49e506b-8c87-44b9-be6c-b9a33f6c9ecb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMCodecProps, IWMCodecProps interface [Media Foundation], IWMCodecProps interface [Media Foundation],described, codecapi.iwmcodecpropsinterface, mf.iwmcodecprops, mf.iwmcodecpropsinterface, wmcodecdsp/IWMCodecProps
ms.topic: interface
req.header: wmcodecdsp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - wmcodecdsp.h
api_name:
 - IWMCodecProps
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMCodecProps interface


## -description


Provides methods that retrieve format-specific codec properties.

This interface is implemented by the video encoder objects. You can obtain a pointer to <a href="https://msdn.microsoft.com/en-us/library/Ff819243(v=VS.85).aspx">IWMCodecProps</a> by calling the <b>QueryInterface</b> method of any other interface on the object, such as <a href="https://msdn.microsoft.com/en-us/library/Dd406926(v=VS.85).aspx">IMediaObject</a> or <a href="https://msdn.microsoft.com/3cc502d8-d364-43b9-b0b6-d9474c002b20">IMFTransform</a>.

This interface enables you to receive information about a specific media type that is supported by a video encoder.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMCodecProps</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMCodecProps</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMCodecProps</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/380c0beb-47a7-46e2-bf5a-cf901d7e0719">GetCodecProp</a>
</td>
<td align="left" width="63%">
Retrieves a codec property.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b9808c67-915c-4767-9107-8d3a38bb9319">GetFormatProp</a>
</td>
<td align="left" width="63%">
Retrieves a format property.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/3e367190-4c88-430e-adbf-9837e1bf0d2b">Media Foundation Interfaces</a>
 

 

