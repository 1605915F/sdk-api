---
UID: NN:strmif.IAMVideoProcAmp
title: IAMVideoProcAmp (strmif.h)
author: windows-sdk-content
description: The IAMVideoProcAmp interface adjusts the qualities of an incoming video signal, such as brightness, contrast, hue, saturation, gamma, and sharpness.The WDM Video Capture filter exposes this interface if the hardware supports image adjustment.
old-location: dshow\iamvideoprocamp.htm
tech.root: DirectShow
ms.assetid: 28c45790-2e5a-4acb-8a53-93f19c51dc6a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAMVideoProcAmp, IAMVideoProcAmp interface [DirectShow], IAMVideoProcAmp interface [DirectShow],described, IAMVideoProcAmpInterface, dshow.iamvideoprocamp, strmif/IAMVideoProcAmp
ms.topic: interface
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IAMVideoProcAmp
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMVideoProcAmp interface


## -description



The <b>IAMVideoProcAmp</b> interface adjusts the qualities of an incoming video signal, such as brightness, contrast, hue, saturation, gamma, and sharpness.

The <a href="https://msdn.microsoft.com/97432b99-e89b-4d69-963d-a959f887e580">WDM Video Capture</a> filter exposes this interface if the hardware supports image adjustment.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAMVideoProcAmp</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IAMVideoProcAmp</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IAMVideoProcAmp</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/8924383e-23e1-4732-9eff-dc7c8d0e361a">Get</a>
</td>
<td align="left" width="63%">
Gets video quality for a specified property.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/54e462a8-bb65-43e2-acf1-f0d64db2bf24">GetRange</a>
</td>
<td align="left" width="63%">
Gets the minimum, maximum, and default values for setting properties.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/18826377-ddf7-4c36-8995-43310ea077dd">Set</a>
</td>
<td align="left" width="63%">
Sets video quality for a specified property.

</td>
</tr>
</table> 


## -remarks



For Windows Driver Model (WDM) devices, the <a href="https://msdn.microsoft.com/97432b99-e89b-4d69-963d-a959f887e580">WDM Video Capture Filter</a> automatically exposes this interface if the WDM driver supports the <a href="https://msdn.microsoft.com/ea1d9c96-b1a5-4849-b607-4c508a526512">PROPSETID_VIDCAP_VIDEOPROCAMP</a> property set. For more information, see the <a href="http://go.microsoft.com/fwlink/p/?linkid=181442">Windows Driver Kit (WDK)</a> documentation.




## -see-also




<a href="https://msdn.microsoft.com/f789db78-292e-4092-a5dc-1906845fb1dd">Configure the Video Quality</a>



<a href="https://msdn.microsoft.com/5efd174f-2eb1-44e6-97e3-b73c7c52fef1">Interfaces</a>
 

 

