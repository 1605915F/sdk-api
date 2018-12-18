---
UID: NN:wmsdkidl.IWMReaderAccelerator
title: IWMReaderAccelerator
author: windows-sdk-content
description: The IWMReaderAccelerator interface is implemented on the reader object only when it is in decoding mode. It is called by a player or a player source filter to obtain interfaces from the decoder DMO.
old-location: wmformat\iwmreaderaccelerator.htm
tech.root: wmformat
ms.assetid: cf783b70-4d19-4006-ad0e-e1f883f00b0b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMReaderAccelerator, IWMReaderAccelerator interface [windows Media Format], IWMReaderAccelerator interface [windows Media Format],described, IWMReaderAcceleratorInterface, wmformat.iwmreaderaccelerator, wmsdkidl/IWMReaderAccelerator
ms.topic: interface
req.header: wmsdkidl.h
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
 - wmsdkidl.h
api_name:
 - IWMReaderAccelerator
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMReaderAccelerator interface


## -description



The <b>IWMReaderAccelerator</b> interface is implemented on the reader object only when it is in decoding mode. It is called by a player or a player source filter to obtain interfaces from the decoder <a href="https://msdn.microsoft.com/en-us/library/Dd757828(v=VS.85).aspx">DMO</a>.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMReaderAccelerator</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMReaderAccelerator</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMReaderAccelerator</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd757427(v=VS.85).aspx">GetCodecInterface</a>
</td>
<td align="left" width="63%">
Retrieves pointers to interfaces exposed on the decoder DMO.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd757428(v=VS.85).aspx">Notify</a>
</td>
<td align="left" width="63%">
Called by the source filter to pass in the negotiated media type.

</td>
</tr>
</table> 

For information about which interfaces can be obtained by using the QueryInterface method of this interface, see <a href="https://msdn.microsoft.com/b5edbf8b-820f-4e09-a482-8efc2283360e">Reader Object</a>.



## -see-also




<a href="https://msdn.microsoft.com/5cb2f564-88e3-4b60-bde3-6ccf69c97c48">Enabling DirectX Video Acceleration</a>
 

 

