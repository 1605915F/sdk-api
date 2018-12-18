---
UID: NF:p2p.PeerCollabStartup
title: PeerCollabStartup function
author: windows-sdk-content
description: Initializes the Peer Collaboration infrastructure.
old-location: p2p\peercollabstartup.htm
tech.root: P2PSdk
ms.assetid: b3f4ac2a-c722-4609-b893-c4b9667ae559
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PeerCollabStartup, PeerCollabStartup function [Peer Networking], p2p.peercollabstartup, p2p/PeerCollabStartup
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
 - PeerCollabStartup
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PeerCollabStartup function


## -description


The <b>PeerCollabStartup</b> function initializes the Peer Collaboration infrastructure.


## -parameters




### -param wVersionRequested [in]

Contains the minimum version of the Peer Collaboration infrastructure requested by the peer.


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
<dt><b>PEER_E_UNSUPPORTED_VERSION</b></dt>
</dl>
</td>
<td width="60%">
The requested version of the Peer Collaboration Infrastructure is not supported.

</td>
</tr>
</table>
 




## -remarks



This function must be called before any other peer collaboration (PeerCollab*) functions are called.

When the application no longer requires the Peer Collaboration infrastructure, it must make a corresponding call to <a href="https://msdn.microsoft.com/4e328188-c8a1-4ba9-817b-3d130a64b985">PeerCollabShutdown</a>. If <b>PeerCollabStartup</b> is called multiple times, there must be a separate corresponding call to <b>PeerCollabShutdown</b>. All of the components of the infrastructure are cleaned up only when the last call to <b>PeerCollabShutdown</b> occurs.

The current supported version is <b>1.0</b>. Call <code>MAKEWORD(1, 0)</code> to generate this version number WORD value.




## -see-also




<a href="https://msdn.microsoft.com/00c3c1f1-c36c-469a-a644-0ec60f02d25e">Peer Collaboration API Functions</a>



<a href="https://msdn.microsoft.com/4e328188-c8a1-4ba9-817b-3d130a64b985">PeerCollabShutdown</a>
 

 

