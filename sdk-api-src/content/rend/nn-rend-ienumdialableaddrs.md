---
UID: NN:rend.IEnumDialableAddrs
title: IEnumDialableAddrs
author: windows-sdk-content
description: The IEnumDialableAddrs interface provides COM-standard enumeration methods to discover and use the available dialable addresses in a directory. The ITDirectoryObject::EnumerateDialableAddrs method returns a pointer to this interface.
old-location: tapi3\ienumdialableaddrs.htm
tech.root: Tapi
ms.assetid: 0a64cb89-9e44-4af1-9b0f-2eec6e5267c7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IEnumDialableAddrs, IEnumDialableAddrs interface [TAPI 2.2], IEnumDialableAddrs interface [TAPI 2.2],described, _tapi3_ienumdialableaddrs, rend/IEnumDialableAddrs, tapi3.ienumdialableaddrs
ms.topic: interface
req.header: rend.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Rend.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Rend.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Rend.dll
api_name:
 - IEnumDialableAddrs
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IEnumDialableAddrs interface


## -description


<p class="CCE_Message">[Rendezvous IP Telephony Conferencing controls and interfaces are not available for use in Windows Vista, Windows Server 2008, and subsequent versions of the operating system. The RTC Client API
provides similar functionality.]

The 
<b>IEnumDialableAddrs</b> interface provides COM-standard enumeration methods to discover and use the available dialable addresses in a directory. The 
<a href="https://msdn.microsoft.com/cee7a00e-e601-47bf-b64b-61085511da97">ITDirectoryObject::EnumerateDialableAddrs</a> method returns a pointer to this interface.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumDialableAddrs</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IEnumDialableAddrs</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEnumDialableAddrs</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/5d05bdfb-007a-451a-bf79-f5a8e4171f85">Clone</a>
</td>
<td align="left" width="63%">
Creates another enumerator that contains the same enumeration state as the current one.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/78ebe1d3-3c40-4ba4-97f0-8612775c80f0">Next</a>
</td>
<td align="left" width="63%">
Gets the next specified number of elements in the enumeration sequence.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c996ea76-bf72-40bd-996b-335448ceb93c">Reset</a>
</td>
<td align="left" width="63%">
Resets to the beginning of the enumeration sequence.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/f68fa12d-dbd3-42a2-bef1-50881d57aa27">Skip</a>
</td>
<td align="left" width="63%">
Skips over the next specified number of elements in the enumeration sequence.

</td>
</tr>
</table> 

