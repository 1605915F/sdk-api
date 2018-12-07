---
UID: NN:segment.IMSVidAudioRendererDevices
title: IMSVidAudioRendererDevices
author: windows-sdk-content
description: The IMSVidAudioRendererDevices interface represents a collection of audio renderers. Applications can use this interface to enumerate the collection. The MSVidAudioRendererDevices object exposes this method.
old-location: mstv\imsvidaudiorendererdevices.htm
tech.root: mstv
ms.assetid: 2cf03260-7abe-4602-8364-447d076a4f76
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMSVidAudioRendererDevices, IMSVidAudioRendererDevices interface [Microsoft TV Technologies], IMSVidAudioRendererDevices interface [Microsoft TV Technologies],described, IMSVidAudioRendererDevicesInterface, mstv.imsvidaudiorendererdevices, segment/IMSVidAudioRendererDevices
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
 - IMSVidAudioRendererDevices
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMSVidAudioRendererDevices interface


## -description



The <b>IMSVidAudioRendererDevices</b> interface represents a collection of audio renderers. Applications can use this interface to enumerate the collection. The <a href="https://msdn.microsoft.com/06a8ddc7-a255-4275-99ed-cb5e3e27c3e0">MSVidAudioRendererDevices</a> object exposes this method.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMSVidAudioRendererDevices</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a> interface. <b>IMSVidAudioRendererDevices</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMSVidAudioRendererDevices</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/663ca24a-9f27-4642-b8e1-901f93090bd7">Add</a>
</td>
<td align="left" width="63%">
Adds an audio renderer to the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/afc8efc7-7e1f-4900-be6b-f41871ad4ebe">get__NewEnum</a>
</td>
<td align="left" width="63%">
Retrieves an enumerator for the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/46a3b579-a027-4c80-9f7a-f81dd9af4d0d">get_Count</a>
</td>
<td align="left" width="63%">
Retrieves the number of items in the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ba6e9161-0881-4f95-9507-acf2a01e05e6">get_Item</a>
</td>
<td align="left" width="63%">
Retrieves the specified item from the collection

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5a9cf752-e3f8-40bf-89e8-e223654e4080">Remove</a>
</td>
<td align="left" width="63%">
Removes an item from the collection.

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IMSVidAudioRendererDevices)</code>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>



<a href="https://msdn.microsoft.com/bf6c3ce9-1e56-4109-93f1-5b313e6ca19b">Video Control Interfaces</a>
 

 

