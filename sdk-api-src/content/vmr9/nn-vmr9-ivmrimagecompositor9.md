---
UID: NN:vmr9.IVMRImageCompositor9
title: IVMRImageCompositor9 (vmr9.h)
author: windows-sdk-content
description: The IVMRImageCompositor9 interface is implemented by the default compositor for the Video Mixing Renderer Filter 9 (VMR-9).
old-location: dshow\ivmrimagecompositor9.htm
tech.root: DirectShow
ms.assetid: 19fda7f2-000f-47d0-a7c7-d8421de418a2
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IVMRImageCompositor9, IVMRImageCompositor9 interface [DirectShow], IVMRImageCompositor9 interface [DirectShow],described, IVMRImageCompositor9Interface, dshow.ivmrimagecompositor9, vmr9/IVMRImageCompositor9
ms.topic: interface
req.header: vmr9.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
 - IVMRImageCompositor9
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVMRImageCompositor9 interface


## -description



The <code>IVMRImageCompositor9</code> interface is implemented by the default compositor for the <a href="https://msdn.microsoft.com/3885cca2-74b1-4066-8ecb-84c9841f9e66">Video Mixing Renderer Filter 9</a> (VMR-9). It must also be implemented by any plug-in compositor that an application provides for the VMR-9. The VMR-9 calls the methods on this interface to inform the compositor that it should composite the incoming video frames into a single output frame. Applications do not use this interface.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IVMRImageCompositor9</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IVMRImageCompositor9</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IVMRImageCompositor9</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd377382(v=VS.85).aspx">CompositeImage</a>
</td>
<td align="left" width="63%">
Composites the current frames available in each input stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd377383(v=VS.85).aspx">InitCompositionDevice</a>
</td>
<td align="left" width="63%">
Informs the compositor that a new composition target has been created.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd377384(v=VS.85).aspx">SetStreamMediaType</a>
</td>
<td align="left" width="63%">
Sets the media type for the input stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd377385(v=VS.85).aspx">TermCompositionDevice</a>
</td>
<td align="left" width="63%">
Informs the compositor that the current composition target is being replaced.

</td>
</tr>
</table> 


## -remarks



Include DShow.h and D3d9.h before Vmr9.h.




## -see-also




<a href="https://msdn.microsoft.com/3d0fdfac-ec7e-4e02-886b-2039c607dac7">Using the Video Mixing Renderer</a>
 

 

