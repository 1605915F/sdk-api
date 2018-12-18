---
UID: NN:wpcapi.IWPCProviderSupport
title: IWPCProviderSupport
author: windows-sdk-content
description: Exposes methods that allow third-party providers to query the currently enabled provider.
old-location: parcon\iwpcprovidersupport.htm
tech.root: parcon
ms.assetid: 5c2a793b-d136-4d03-9e46-b24009af2c7d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWPCProviderSupport, IWPCProviderSupport interface, IWPCProviderSupport interface,described, parcon.iwpcprovidersupport, wpcapi/IWPCProviderSupport
ms.topic: interface
req.header: wpcapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
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
 - Wpcapi.h
api_name:
 - IWPCProviderSupport
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWPCProviderSupport interface


## -description


Exposes methods that allow third-party providers to query the currently enabled provider.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWPCProviderSupport</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWPCProviderSupport</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWPCProviderSupport</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/36496cba-229c-45bb-9608-04fb4b1955ae">GetCurrent</a>
</td>
<td align="left" width="63%">
Retrieves the GUID of the current provider.

</td>
</tr>
</table> 

