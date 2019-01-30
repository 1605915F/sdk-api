---
UID: NN:strmif.IEnumStreamIdMap
title: IEnumStreamIdMap
author: windows-sdk-content
description: The IEnumStreamIdMap interface is implemented on a standard COM collection of Stream ID maps that have been created by the MPEG-2 Demultiplexer's IMPEG2StreamIdMap::MapStreamId method.
old-location: dshow\ienumstreamidmap.htm
tech.root: DirectShow
ms.assetid: 8bca9255-2bc8-408b-9127-e3fe050fcf01
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumStreamIdMap, IEnumStreamIdMap interface [DirectShow], IEnumStreamIdMap interface [DirectShow],described, IEnumStreamIdMapInterface, dshow.ienumstreamidmap, strmif/IEnumStreamIdMap
ms.topic: interface
req.header: strmif.h
req.include-header: Dshow.h
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
 - IEnumStreamIdMap
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumStreamIdMap interface


## -description



The <code>IEnumStreamIdMap</code> interface is implemented on a standard COM collection of Stream ID maps that have been created by the <a href="https://msdn.microsoft.com/99bfc55d-6519-4e85-98ce-cad27bd71ffb">MPEG-2 Demultiplexer</a>'s <a href="https://msdn.microsoft.com/e74a1e62-1bc4-43e1-9017-85012b2ece01">IMPEG2StreamIdMap::MapStreamId</a> method. To obtain a pointer to this interface, use the <a href="https://msdn.microsoft.com/2c42f042-c9fb-4cb9-90bb-4050a61b18da">IMPEG2StreamIdMap::EnumStreamIdMap</a> method. Typically, an output pin will never have more than one stream ID mapped to it at any given time. This collection represents a snapshot of the Stream IDs mapped at the time the collection is created. The collection is not updated automatically.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumStreamIdMap</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IEnumStreamIdMap</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEnumStreamIdMap</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2c6ef2a8-a5d7-434f-8de2-221502b7c5cf">Clone</a>
</td>
<td align="left" width="63%">
Creates a new copy of the collection and all its sub-objects.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/49e7ab23-e57e-4437-a195-88bccb6002de">Next</a>
</td>
<td align="left" width="63%">
Retrieves the next <i>n</i> elements in the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2e8bc22c-8a13-4a5a-a15d-af4e1ed699bd">Reset</a>
</td>
<td align="left" width="63%">
Moves the iterator to the beginning of the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/54502cd5-50b2-4bd2-a13f-180bddac178a">Skip</a>
</td>
<td align="left" width="63%">
Skips over the specified element in the collection.

</td>
</tr>
</table> 

