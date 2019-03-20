---
UID: NN:callobj.ICallUnmarshal
title: ICallUnmarshal (callobj.h)
author: windows-sdk-content
description: Is used on the server (receiving) side of a remote invocation.
old-location: com\icallunmarshal.htm
tech.root: com
ms.assetid: 66de8d71-c27c-41bd-a741-02de5c779290
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICallUnmarshal, ICallUnmarshal interface [COM], ICallUnmarshal interface [COM],described, _com_icallunmarshal_interface, callobj/ICallUnmarshal, com.icallunmarshal
ms.topic: interface
req.header: callobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Callobj.idl
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
 - Callobj.h
api_name:
 - ICallUnmarshal
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICallUnmarshal interface


## -description


Is used on the server (receiving) side of a remote invocation. An appropriate instance of <b>ICallUnmarshal</b> can be used to transform back into an call frame a method invocation previously marshaled by a call to <a href="https://msdn.microsoft.com/cab40c31-1f89-4da9-a1e0-ef946b34665c">ICallFrame::Marshal</a> on the client (sending) side. After such a reconstituted call frame is obtained, the call can be carried out on an actual object using <a href="https://msdn.microsoft.com/75cb7b96-55c9-4aee-b507-a549e2af38bc">ICallFrame::Invoke</a>.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ICallUnmarshal</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>ICallUnmarshal</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ICallUnmarshal</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c7b1aff8-338a-491a-908f-5f85dddd89b7">ReleaseMarshalData</a>
</td>
<td align="left" width="63%">
Releases resources that may be held by interface pointers residing in a packet of marshaled data.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/15d04287-285d-43d9-ad55-3dc9c7ae192e">Unmarshal</a>
</td>
<td align="left" width="63%">
Turns a marshaled packet of data back into an activation record that can then be invoked or manipulated in some other way.

</td>
</tr>
</table> 

