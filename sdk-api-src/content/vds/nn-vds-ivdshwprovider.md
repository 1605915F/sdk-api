---
UID: NN:vds.IVdsHwProvider
title: IVdsHwProvider
author: windows-sdk-content
description: Provides methods for performing query, reenumeration, and refresh operations on a hardware provider.
old-location: base\ivdshwprovider.htm
tech.root: VDS
ms.assetid: ff90875d-f437-4236-a13f-d55a83b778b9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IVdsHwProvider, IVdsHwProvider interface [VDS], IVdsHwProvider interface [VDS],described, base.ivdshwprovider, vds/IVdsHwProvider, vdshwprv/IVdsHwProvider
ms.topic: interface
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.lib: Uuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Uuid.lib
 - Uuid.dll
api_name:
 - IVdsHwProvider
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IVdsHwProvider interface


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Provides methods for 
   performing query, reenumeration, and refresh operations on a hardware provider.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IVdsHwProvider</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IVdsHwProvider</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IVdsHwProvider</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ae327655-3db9-44b0-934a-458ee90b1d07">QuerySubSystems</a>
</td>
<td align="left" width="63%">
Returns an enumeration of the subsystems managed by the provider.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/aeb06a98-8896-446f-abd5-ea40be0bea40">Reenumerate</a>
</td>
<td align="left" width="63%">
Discovers newly connected and disconnected subsystems.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/25ddc73c-5d1b-4bec-bbc2-9f22a5f82ffe">Refresh</a>
</td>
<td align="left" width="63%">
Refreshes the internally-cached data about existing subsystems managed by the provider.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/55171eb1-6fec-4651-914c-88d23e8d7849">IVdsService::QueryProviders</a>



<a href="https://msdn.microsoft.com/131e927d-d32a-44f6-8aae-28839cfa9e7d">Provider Object</a>



<a href="https://msdn.microsoft.com/0bddfd62-881d-4fda-b303-ed38d434af55">VDS Interfaces</a>
 

 

