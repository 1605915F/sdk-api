---
UID: NS:madcapcl._MCAST_LEASE_REQUEST
title: MCAST_LEASE_REQUEST
author: windows-sdk-content
description: The MCAST_LEASE_REQUEST structure defines the request, renew, or release parameters for a given multicast scope. In the MCAST_API_VERSION_1 implementation, only one IP address may be allocated at a time.
old-location: madcap\mcast_lease_request.htm
tech.root: Madcap
ms.assetid: 3110a1f3-e252-4eab-bf69-cbecfd65a5e0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMCAST_LEASE_REQUEST, MCAST_LEASE_REQUEST, MCAST_LEASE_REQUEST structure [MADCAP], PMCAST_LEASE_REQUEST, PMCAST_LEASE_REQUEST structure pointer [MADCAP], _mdhcp_mcast_lease_request, madcap.mcast_lease_request, madcapcl/MCAST_LEASE_REQUEST, madcapcl/PMCAST_LEASE_REQUEST"
ms.topic: struct
req.header: madcapcl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - HeaderDef
api_location:
 - Madcapcl.h
api_name:
 - MCAST_LEASE_REQUEST
product: Windows
targetos: Windows
req.typenames: MCAST_LEASE_REQUEST, *PMCAST_LEASE_REQUEST
req.redist: 
---

# MCAST_LEASE_REQUEST structure


## -description


The 
<b>MCAST_LEASE_REQUEST</b> structure defines the request, renew, or release parameters for a given multicast scope. In the MCAST_API_VERSION_1 implementation, only one IP address may be allocated at a time.


## -struct-fields




### -field LeaseStartTime

Requested start time, in seconds, for the multicast scope lease elapsed since midnight of January 1, 1970, coordinated universal time. To request the current time as the lease start time, set <b>LeaseStartTime</b> to zero.


### -field MaxLeaseStartTime

Maximum start time, in seconds, elapsed since midnight of January 1, 1970, coordinated universal time, that the client is willing to accept.


### -field LeaseDuration

Duration of the lease request, in seconds. To request the default lease duration, set both <b>LeaseDuration</b> and <b>MinLeaseDuration</b> to zero.


### -field MinLeaseDuration

Minimum lease duration, in seconds, that the client is willing to accept.


### -field ServerAddress

Internet Protocol (IP) address of the server on which the lease is to be requested or renewed, in the form of an 
<a href="https://msdn.microsoft.com/c3dc76aa-d903-49be-a4a2-1f66cafff40a">IPNG_ADDRESS</a> structure. If the IP address of the server is unknown, such as when using this structure in an 
<a href="https://msdn.microsoft.com/856eb251-1909-41a1-8e4f-c081942280de">McastRequestAddress</a> function call, set <b>ServerAddress</b> to zero.


### -field MinAddrCount

Minimum number of IP addresses the client is willing to accept.


### -field AddrCount

Number of requested IP addresses. Note that the value of this member dictates the size of <b>pAddrBuf</b>.


### -field pAddrBuf

Pointer to a buffer containing the requested IP addresses. For IPv4 addresses, the <b>pAddrBuf</b> member points to 4-byte addresses; for IPv6 addresses, the <b>pAddrBuf</b> member points to 16-byte addresses. If no specific addresses are requested, set <b>pAddrBuf</b> to <b>NULL</b>.


## -remarks



In MCAST_API_VERSION_1 version, <b>MaxLeaseStartTime</b>, <b>MinLeaseDuration</b>, and <b>MinAddrCount</b> members are ignored. Clients should still set appropriate values for these members, however, to take advantage of their implementation in future updates.




## -see-also




<a href="https://msdn.microsoft.com/c3dc76aa-d903-49be-a4a2-1f66cafff40a">IPNG_ADDRESS</a>



<a href="https://msdn.microsoft.com/6460ea80-f1b1-4939-a977-580d0db10fd0">MCAST_CLIENT_UID</a>



<a href="https://msdn.microsoft.com/1993e3bc-b6bd-4e13-aa71-7e33bf7ef540">MCAST_LEASE_RESPONSE</a>



<a href="https://msdn.microsoft.com/164d8f73-f5f5-4cc6-85ca-8e249192c202">MCAST_SCOPE_CTX</a>



<a href="https://msdn.microsoft.com/d275e78b-ddf3-4f92-a76f-463aec2f6c95">MCAST_SCOPE_ENTRY</a>



<a href="https://msdn.microsoft.com/eccf52ee-8145-4a8f-9d34-5a56bfc8a48c">McastApiCleanup</a>



<a href="https://msdn.microsoft.com/edb7d666-cbd0-46f7-b63e-2a09ffc9e9e2">McastApiStartup</a>



<a href="https://msdn.microsoft.com/df33d766-d420-4069-8b94-86f5e4e91c1d">McastEnumerateScopes</a>



<a href="https://msdn.microsoft.com/67d5f149-d9b3-4903-a859-1ad33e310997">McastGenUID</a>



<a href="https://msdn.microsoft.com/856eb251-1909-41a1-8e4f-c081942280de">McastRequestAddress</a>
 

 

