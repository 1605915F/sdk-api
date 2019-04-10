---
UID: NN:wpcapi.IWPCProviderState
title: IWPCProviderState (wpcapi.h)
author: windows-sdk-content
description: Exposes provider state methods that are implemented by third parties.
old-location: parcon\iwpcproviderstate.htm
tech.root: parcon
ms.assetid: a5cd14df-8e64-4f34-801c-9901c7d215f9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWPCProviderState, IWPCProviderState interface, IWPCProviderState interface,described, parcon.iwpcproviderstate, wpcapi/IWPCProviderState
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
req.idl: Wpcprovider.idl
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
 - IWPCProviderState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWPCProviderState interface


## -description


Exposes provider state methods that are implemented by third parties.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWPCProviderState</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWPCProviderState</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWPCProviderState</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/2aa1a236-b681-4226-a337-507d0854955d">Disable</a>
</td>
<td align="left" width="63%">
Notifies the third-party application that it is not the current provider.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6714702d-e623-43f8-9a4e-dd1b3939d011">Enable</a>
</td>
<td align="left" width="63%">
Notifies the third-party application that it has been selected as the new current provider.

</td>
</tr>
</table> 

