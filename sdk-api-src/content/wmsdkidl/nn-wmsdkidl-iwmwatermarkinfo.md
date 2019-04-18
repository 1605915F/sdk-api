---
UID: NN:wmsdkidl.IWMWatermarkInfo
title: IWMWatermarkInfo (wmsdkidl.h)
author: windows-sdk-content
description: The IWMWatermarkInfo interface retrieves information about available watermarking systems.
old-location: wmformat\iwmwatermarkinfo.htm
tech.root: wmformat
ms.assetid: 4bdad433-31d1-442c-9701-f3748245070d
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWMWatermarkInfo, IWMWatermarkInfo interface [windows Media Format], IWMWatermarkInfo interface [windows Media Format],described, IWMWatermarkInfoInterface, wmformat.iwmwatermarkinfo, wmsdkidl/IWMWatermarkInfo
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
 - IWMWatermarkInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWMWatermarkInfo interface


## -description



The <b>IWMWatermarkInfo</b> interface retrieves information about available watermarking systems. Watermarking systems are implemented in DirectX Media Objects that are registered for use with the Windows Media Formats SDK.

An <b>IWMWatermarkInfo</b> interface exists for every writer object. To obtain a pointer to this interface, call <b>QueryInterface</b> on any other interface of the writer object.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMWatermarkInfo</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMWatermarkInfo</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMWatermarkInfo</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd798717(v=VS.85).aspx">GetWatermarkEntry</a>
</td>
<td align="left" width="63%">
Retrieves information about one available watermarking system.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd798718(v=VS.85).aspx">GetWatermarkEntryCount</a>
</td>
<td align="left" width="63%">
Retrieves the total number of watermarking systems available.

</td>
</tr>
</table> 

For information about which interfaces can be obtained by using the QueryInterface method of this interface, see <a href="https://msdn.microsoft.com/8058b7fe-7d02-4572-ad43-6867d4ceb7e9">Writer Object</a>.



## -see-also




<a href="https://msdn.microsoft.com/c61a0739-09f2-497f-a2cd-d3f2472738e3">Interfaces</a>



<a href="https://msdn.microsoft.com/1fafb15e-57b8-4dd0-8f0c-ccf460f05157">Watermarking Support</a>
 

 

