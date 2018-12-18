---
UID: NN:austream.IAudioData
title: IAudioData
author: windows-sdk-content
description: Note  This interface is deprecated.
old-location: dshow\iaudiodata.htm
tech.root: DirectShow
ms.assetid: 8b253715-a294-4e95-b730-e6efe7f895af
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IAudioData, IAudioData interface [DirectShow], IAudioData interface [DirectShow],described, IAudioDataInterface, austream/IAudioData, dshow.iaudiodata
ms.topic: interface
req.header: austream.h
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
 - austream.h
api_name:
 - IAudioData
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IAudioData interface


## -description



<div class="alert"><b>Note</b>  This interface is deprecated. New applications should not use it.</div>
<div> </div>
The <code>IAudioData</code> interface provides methods that enable applications to set and get the underlying audio data that audio streams will reference. The audio data format is set in the <a href="https://msdn.microsoft.com/4f3bf6fb-b15f-43b3-82f1-e7a8a3007057">WAVEFORMATEX</a> structure.

Implement this interface on underlying audio data objects that audio stream sample objects will access.

Applications use this interface to set and retrieve information on underlying data objects that an audio stream will reference.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IAudioData</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Dd407080(v=VS.85).aspx">IMemoryData</a>. <b>IAudioData</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IAudioData</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd389514(v=VS.85).aspx">GetFormat</a>
</td>
<td align="left" width="63%">
Retrieves the current data format.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd389515(v=VS.85).aspx">SetFormat</a>
</td>
<td align="left" width="63%">
Sets the current data format.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd407080(v=VS.85).aspx">IMemoryData</a>
 

 

