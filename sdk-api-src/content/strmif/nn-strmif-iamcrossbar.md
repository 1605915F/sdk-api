---
UID: NN:strmif.IAMCrossbar
title: IAMCrossbar (strmif.h)
author: windows-sdk-content
description: The IAMCrossbar interface routes signals from an analog or digital source to a video capture filter.This interface is implemented by the Analog Video Crossbar Filter.
old-location: dshow\iamcrossbar.htm
tech.root: DirectShow
ms.assetid: 9eef4923-62e7-475e-85e6-de8c1eefe483
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAMCrossbar, IAMCrossbar interface [DirectShow], IAMCrossbar interface [DirectShow],described, IAMCrossbarInterface, dshow.iamcrossbar, strmif/IAMCrossbar
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
 - IAMCrossbar
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAMCrossbar interface


## -description



The <code>IAMCrossbar</code> interface routes signals from an analog or digital source to a video capture filter.

This interface is implemented by the <a href="https://msdn.microsoft.com/668f6a8b-a4ed-4e4a-956c-a87f165225fa">Analog Video Crossbar Filter</a>. The Analog Video Crossbar filter is modeled after a general switching matrix, with <i>n</i> inputs and <i>m</i> outputs. For example, a video card might have two external connectors: a coaxial connector for TV, and an S-video input. These would be represented as input pins on the filter. To select one of the inputs, an application would use the <code>IAMCrossbar</code> interface to "route" an input pin to the filter's output pin, by calling the <a href="https://msdn.microsoft.com/a3f6823d-e389-478a-b882-2556a3cbd821">IAMCrossbar::Route</a> method.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAMCrossbar</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IAMCrossbar</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IAMCrossbar</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/13be4b35-14d9-4565-8939-e6e755f256ab">CanRoute</a>
</td>
<td align="left" width="63%">
Queries whether a specified input pin can be routed to a specified output pin.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/29cda12e-a731-4995-8e0c-69dfcda6f158">get_CrossbarPinInfo</a>
</td>
<td align="left" width="63%">
Retrieves information about a specified pin.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/fbd59205-ef0a-4e1c-b9d3-63a083c0a7f6">get_IsRoutedTo</a>
</td>
<td align="left" width="63%">
Retrieves the input pin that is currently routed to the specified output pin.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/66ea86a6-82c3-4f91-a2d3-a08014f555be">get_PinCounts</a>
</td>
<td align="left" width="63%">
Retrieves the number of input and output pins on the crossbar filter.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/a3f6823d-e389-478a-b882-2556a3cbd821">Route</a>
</td>
<td align="left" width="63%">
Routes an input pin to an output pin.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/6e8ee9c3-6776-498b-ad38-36f8172a27ae">Working with Crossbars</a>
 

 

