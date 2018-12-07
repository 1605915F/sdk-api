---
UID: NN:mileffects.IMILBitmapEffectConnector
title: IMILBitmapEffectConnector
author: windows-sdk-content
description: Exposes methods that define an effect output pin.
old-location: wibe\_wibe_imilbitmapeffectconnector.htm
tech.root: wibe
ms.assetid: VS|wibe|~\wibelh\reference\ifaces\imilbitmapeffectconnector\imilbitmapeffectconnector.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMILBitmapEffectConnector, IMILBitmapEffectConnector interface [WPF Bitmap Effects], IMILBitmapEffectConnector interface [WPF Bitmap Effects],described, _wibe_imilbitmapeffectconnector, mileffects/IMILBitmapEffectConnector, wibe._wibe_imilbitmapeffectconnector
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: mileffects.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mileffects.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Mileffects.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mileffects.dll
api_name:
 - IMILBitmapEffectConnector
product: Windows
targetos: Windows
req.typenames: 
req.redist: Microsoft .Net 3.0
---

# IMILBitmapEffectConnector interface


## -description


Exposes methods that define an effect output pin.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMILBitmapEffectConnector</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IMILBitmapEffectConnector</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMILBitmapEffectConnector</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms735304(v=VS.85).aspx">GetBitmapEffect</a>
</td>
<td align="left" width="63%">
Gets the <a href="https://msdn.microsoft.com/en-us/library/ms735317(v=VS.85).aspx">IMILBitmapEffect</a> associated with the connector.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/ms735306(v=VS.85).aspx">IsConnected</a>
</td>
<td align="left" width="63%">
Determines whether the connector is connected to an effect.

</td>
</tr>
</table> 

