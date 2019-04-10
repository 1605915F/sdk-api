---
UID: NF:p2p.PeerCollabGetInvitationResponse
title: PeerCollabGetInvitationResponse function (p2p.h)
author: windows-sdk-content
description: Obtains the response from a peer previously invited to join a peer collaboration activity.
old-location: p2p\peercollabgetinvitationresponse.htm
tech.root: P2PSdk
ms.assetid: f9471e51-5eec-4927-bd12-7d362f5101ee
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: PeerCollabGetInvitationResponse, PeerCollabGetInvitationResponse function [Peer Networking], p2p.peercollabgetinvitationresponse, p2p/PeerCollabGetInvitationResponse
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
 - PeerCollabGetInvitationResponse
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PeerCollabGetInvitationResponse function


## -description


The <b>PeerCollabGetInvitationResponse</b> function obtains the response from  a peer previously invited to join a peer collaboration activity.


## -parameters




### -param hInvitation [in]

Handle to an invitation to join a peer collaboration activity.


### -param ppInvitationResponse [out]

Pointer to the address of a <a href="https://msdn.microsoft.com/9f77c471-ef05-442f-aeae-afe67319b0ff">PEER_INVITATION_RESPONSE</a> structure that contains an invited peer's response to a previously transmitted invitation request.

Free the memory associated with this structure by calling <a href="https://msdn.microsoft.com/54288829-c991-42d6-a7c4-874ed28dd106">PeerFreeData</a>.


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
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The provided handle is invalid.

</td>
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
<dt><b>PEER_E_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The invitation recipient could not be found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PEER_E_INVITE_CANCELED</b></dt>
</dl>
</td>
<td width="60%">
The invitation was previously canceled.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PEER_E_INVITE_RESPONSE_NOT_AVAILABLE</b></dt>
</dl>
</td>
<td width="60%">
The response to the peer invitation is not available.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>PEER_E_CONNECTION_FAILED</b></dt>
</dl>
</td>
<td width="60%">
A connection to the graph or group has failed, or a direct connection in a graph or group has failed.

</td>
</tr>
</table>
 




## -remarks



This function must be called after <a href="https://msdn.microsoft.com/2101e16e-ee05-417f-835b-c00cba7f6576">PeerCollabAsyncInviteContact</a> or <a href="https://msdn.microsoft.com/2606d2ef-26d3-4c52-b481-3ea38350295a">PeerCollabAsyncInviteEndpoint</a> is called and the event handle provided to <a href="https://msdn.microsoft.com/en-us/library/Aa371077(v=VS.85).aspx">PeerCollabRegisterEvent</a> is signaled on the peer that sent the invitation.




## -see-also




<a href="https://msdn.microsoft.com/9f77c471-ef05-442f-aeae-afe67319b0ff">PEER_INVITATION_RESPONSE</a>



<a href="https://msdn.microsoft.com/00c3c1f1-c36c-469a-a644-0ec60f02d25e">Peer Collaboration API Functions</a>



<a href="https://msdn.microsoft.com/2101e16e-ee05-417f-835b-c00cba7f6576">PeerCollabAsyncInviteContact</a>



<a href="https://msdn.microsoft.com/2606d2ef-26d3-4c52-b481-3ea38350295a">PeerCollabAsyncInviteEndpoint</a>
 

 

