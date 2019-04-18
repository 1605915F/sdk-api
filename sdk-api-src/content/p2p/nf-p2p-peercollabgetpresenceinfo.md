---
UID: NF:p2p.PeerCollabGetPresenceInfo
title: PeerCollabGetPresenceInfo function (p2p.h)
author: windows-sdk-content
description: Retrieves the presence information for the endpoint associated with a specific contact.
old-location: p2p\peercollabgetpresenceinfo.htm
tech.root: P2PSdk
ms.assetid: 596191a1-94cf-4497-aaf0-951e2c63b145
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: PeerCollabGetPresenceInfo, PeerCollabGetPresenceInfo function [Peer Networking], p2p.peercollabgetpresenceinfo, p2p/PeerCollabGetPresenceInfo
ms.topic: function
req.header: p2p.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.lib: P2P.lib
req.dll: P2P.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - P2P.dll
api_name:
 - PeerCollabGetPresenceInfo
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# PeerCollabGetPresenceInfo function


## -description


The <b>PeerCollabGetPresenceInfo</b> function retrieves the  presence information for the endpoint associated with a specific contact.


## -parameters




### -param pcEndpoint [in]

Pointer to a <a href="https://msdn.microsoft.com/9687b332-14ed-4023-b8c2-437d75fd0298">PEER_ENDPOINT</a> structure that contains the specific endpoint associated with the contact specified in <i>pcContact</i> for which presence information must be returned.


### -param ppPresenceInfo [out]

Pointer  to the address of the <a href="https://msdn.microsoft.com/e8f83ba8-81a3-4083-bc15-e00b2bec1cd4">PEER_PRESENCE_INFO</a> structure that contains the requested presence data for the supplied endpoint.


## -returns



Returns S_OK if the function succeeds. Otherwise, the function returns one of the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
There is not enough memory to support this operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
One of the arguments is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PEER_E_NOT_INITIALIZED</b></dt>
</dl>
</td>
<td width="60%">
The application did not make a previous call to <a href="https://msdn.microsoft.com/b3f4ac2a-c722-4609-b893-c4b9667ae559">PeerCollabStartup</a>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PEER_E_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The presence information for the specified endpoint was not found in the peer collaboration network.

</td>
</tr>
</table>
 




## -remarks



To obtain a peer object successfully:<ul>
<li>The endpoint must have been previously obtained by calling <a href="https://msdn.microsoft.com/c29d089c-1f1e-4d50-9a3a-18c844b4ad1c">PeerCollabEnumEndpoints</a>.
</li>
<li>The local peer must have subscribed to the endpoint by calling <a href="https://msdn.microsoft.com/dfe17235-34dd-4694-9ee5-4268b4406731">PeerCollabSubscribeEndpointData</a>.</li>
<li>The endpoint data must be refreshed by calling <a href="https://msdn.microsoft.com/ba841da4-de7f-4288-84b7-a06370b55e3c">PeerCollabRefreshEndpointData</a> successfully.</li>
</ul>





## -see-also




<a href="https://msdn.microsoft.com/b84a17fc-35d6-4098-9bb3-18e708541a80">PEER_CONTACT</a>



<a href="https://msdn.microsoft.com/9687b332-14ed-4023-b8c2-437d75fd0298">PEER_ENDPOINT</a>



<a href="https://msdn.microsoft.com/e8f83ba8-81a3-4083-bc15-e00b2bec1cd4">PEER_PRESENCE_INFO</a>



<a href="https://msdn.microsoft.com/00c3c1f1-c36c-469a-a644-0ec60f02d25e">Peer Collaboration API Functions</a>
 

 

