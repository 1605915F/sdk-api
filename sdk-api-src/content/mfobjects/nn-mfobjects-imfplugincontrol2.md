---
UID: NN:mfobjects.IMFPluginControl2
title: IMFPluginControl2
author: windows-sdk-content
description: Controls how media sources and transforms are enumerated in Microsoft Media Foundation.
old-location: mf\imfplugincontrol2.htm
tech.root: medfound
ms.assetid: 15BD57FC-7CEF-45DC-AF94-3E54A3A9477A
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMFPluginControl2, IMFPluginControl2 interface [Media Foundation], IMFPluginControl2 interface [Media Foundation],described, mf.imfplugincontrol2, mfobjects/IMFPluginControl2
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: mfobjects.h
req.include-header: Mfidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - mfobjects.h
api_name:
 - IMFPluginControl2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFPluginControl2 interface


## -description


Controls how media sources and transforms are enumerated in Microsoft Media Foundation.

This interface extends the <a href="https://msdn.microsoft.com/cdc6fd4f-c544-43bb-ba99-5468ef49949d">IMFPluginControl</a> interface.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMFPluginControl2</b> interface inherits from <a href="https://msdn.microsoft.com/cdc6fd4f-c544-43bb-ba99-5468ef49949d">IMFPluginControl</a>. <b>IMFPluginControl2</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMFPluginControl2</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/1B078EB2-D87E-46A4-B2E1-A850C4E543A8">SetPolicy</a>
</td>
<td align="left" width="63%">
Sets the policy for which media sources and transforms are enumerated.

</td>
</tr>
</table> 


## -remarks



To get a pointer to this interface, call <a href="https://msdn.microsoft.com/68b25c68-806d-46c3-98f8-8f29d7c21471">MFGetPluginControl</a>  and query the returned pointer for <b>IMFPluginControl2</b>.




## -see-also




<a href="https://msdn.microsoft.com/cdc6fd4f-c544-43bb-ba99-5468ef49949d">IMFPluginControl</a>



<a href="https://msdn.microsoft.com/3e367190-4c88-430e-adbf-9837e1bf0d2b">Media Foundation Interfaces</a>
 

 

