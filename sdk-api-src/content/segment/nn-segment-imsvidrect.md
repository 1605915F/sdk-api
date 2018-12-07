---
UID: NN:segment.IMSVidRect
title: IMSVidRect
author: windows-sdk-content
description: The IMSVidRect interface represents a rectangle with an associated window handle.
old-location: mstv\imsvidrect.htm
tech.root: mstv
ms.assetid: 0b3cf31b-e0cc-4208-a128-b77460fc0f1b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidRect, IMSVidRect interface [Microsoft TV Technologies], IMSVidRect interface [Microsoft TV Technologies],described, IMSVidRectInterface, mstv.imsvidrect, segment/IMSVidRect
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Segment.idl
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
 - segment.h
api_name:
 - IMSVidRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidRect interface


## -description



The <b>IMSVidRect</b> interface represents a rectangle with an associated window handle. It contains methods to set and retrieve the top and left coordinates, the width, and the height. All values are in pixels. The top and left coordinates are relative to the associated window.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMSVidRect</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IMSVidRect</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMSVidRect</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/83925bca-8cb2-4f79-9aca-1bee0fb4a96a">get_Height</a>
</td>
<td align="left" width="63%">
Retrieves the height of the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/caa56beb-7eba-48a1-8645-f63666ba0593">get_HWnd</a>
</td>
<td align="left" width="63%">
Retrieves the window associated with the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/9e64e560-033b-475a-a281-57af5f893e65">get_Left</a>
</td>
<td align="left" width="63%">
Retrieves the left x-coordinate of the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/3596141c-e359-4ea5-8d6a-9ec374c1f854">get_Top</a>
</td>
<td align="left" width="63%">
Retrieves the top y-coordinate of the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7b1d07b8-41e4-44f8-8c28-377c7a9e463d">get_Width</a>
</td>
<td align="left" width="63%">
Retrieves the width of the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/410c5d1c-d4e6-460a-b17d-54bfcee10a66">put_Height</a>
</td>
<td align="left" width="63%">
Specifies the height of the rectangle

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/bbc7a6d0-2829-4fdb-89da-5ebb7fc803eb">put_HWnd</a>
</td>
<td align="left" width="63%">
Specifies the window associated with the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/8e61fd8a-9ea0-48c1-8749-780b0363c12d">put_Left</a>
</td>
<td align="left" width="63%">
Specifies the left x-coordinate of the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/e50fd657-d913-49f5-b4dd-fb4c0d207417">put_Rect</a>
</td>
<td align="left" width="63%">
Copies the values of another rectangle to this rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ee3dbbd2-a8b4-496b-84e6-b0d7615f6a1e">put_Top</a>
</td>
<td align="left" width="63%">
Specifies the top y-coordinate of the rectangle.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/35eed36a-de3e-4bb6-8b1b-179ba72b568a">put_Width</a>
</td>
<td align="left" width="63%">
Specifies the width of the rectangle.

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IMSVidRect)</code>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>



<a href="https://msdn.microsoft.com/bf6c3ce9-1e56-4109-93f1-5b313e6ca19b">Video Control Interfaces</a>
 

 

