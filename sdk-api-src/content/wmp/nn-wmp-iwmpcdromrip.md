---
UID: NN:wmp.IWMPCdromRip
title: IWMPCdromRip
author: windows-sdk-content
description: The IWMPCdromRip interface provides methods to manage copying, or ripping, tracks from an audio CD.Ripping a CD by using the IWMPCdromRip interface has the same effect as ripping music by using the Windows Media Player user interface.
old-location: wmp\iwmpcdromrip.htm
tech.root: WMP
ms.assetid: c3e2db46-bef0-4c79-91b5-97ca5a86c6ba
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMPCdromRip, IWMPCdromRip interface [Windows Media Player], IWMPCdromRip interface [Windows Media Player],described, IWMPCdromRipInterface, wmp.iwmpcdromrip, wmp/IWMPCdromRip
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: wmp.h
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
 - wmp.h
api_name:
 - IWMPCdromRip
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMPCdromRip interface


## -description



The <b>IWMPCdromRip</b> interface provides methods to manage copying, or <i>ripping</i>, tracks from an audio CD.

Ripping a CD by using the <b>IWMPCdromRip</b> interface has the same effect as ripping music by using the Windows Media Player user interface. Ripped content is automatically added to the library according to the user's preferences. For more information about user preferences for CD ripping, see "Ripping music from CDs" in Windows Media Player Help.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWMPCdromRip</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWMPCdromRip</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWMPCdromRip</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/d7140bc9-bf79-48f0-aaf0-155660c8b2c9">get_ripProgress</a>
</td>
<td align="left" width="63%">
Retrieves the CD ripping progress as percent complete.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/81c7ba1d-81d7-4f64-9f7d-c88d6959bee0">get_ripState</a>
</td>
<td align="left" width="63%">
Retrieves an enumeration value that indicates the current state of the ripping process.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/88ba1e83-a3c5-4922-8c58-37993ccb4afc">startRip</a>
</td>
<td align="left" width="63%">
Rips the CD.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2a6c5a25-f69c-4258-a92f-7f693b201a01">stopRip</a>
</td>
<td align="left" width="63%">
Stops the CD ripping process.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/68a0bdaf-ae1b-4ba1-817b-a31c68b9fddd">Interfaces</a>



<a href="https://msdn.microsoft.com/f5c1b5bf-d616-48cb-8690-e0237c56e402">Ripping a CD</a>
 

 

