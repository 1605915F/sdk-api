---
UID: NF:netioapi.ResolveIpNetEntry2
title: ResolveIpNetEntry2 function
author: windows-sdk-content
description: Resolves the physical address for a neighbor IP address entry on the local computer.
old-location: iphlp\resolveipnetentry2.htm
tech.root: IpHlp
ms.assetid: 37f9dc58-362d-413e-a593-4dda52fb7d8b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ResolveIpNetEntry2, ResolveIpNetEntry2 function [IP Helper], iphlp.resolveipnetentry2, netioapi/ResolveIpNetEntry2
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: netioapi.h
req.include-header: Iphlpapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Iphlpapi.lib
req.dll: Iphlpapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Iphlpapi.dll
api_name:
 - ResolveIpNetEntry2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResolveIpNetEntry2 function


## -description


The 
<b>ResolveIpNetEntry2</b> function  resolves the physical address for a neighbor IP address entry on the local computer. 


## -parameters




### -param Row [in, out]

A pointer to a 
<a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a> structure entry for a neighbor IP address entry. On successful return, this structure will be updated with the properties for neighbor IP address.


### -param SourceAddress [in, optional]

A pointer to a 
an optional source IP address used to select the interface to send the requests on for the neighbor IP address entry. 


## -returns



If the function succeeds, the return value is NO_ERROR.

If the function fails, the return value is one of the following error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_BAD_NET_NAME</b></dt>
</dl>
</td>
<td width="60%">
The network name cannot be found. This error is returned if the network with the neighbor IP address is unreachable.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
An invalid parameter was passed to the function. This error is returned if a <b>NULL</b> pointer is passed in the <i>Row</i> parameter, the <b>Address</b> member of the <a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a> pointed to by the <i>Row</i> parameter was not set to a valid IPv4 or IPv6 address, or both the <b>InterfaceLuid</b> or <b>InterfaceIndex</b> members of the <b>MIB_IPNET_ROW2</b> pointed to by the <i>Row</i> parameter were unspecified. This error is also returned if a loopback address was passed in the <b>Address</b> member. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The specified interface could not be found. This error is returned if the  network interface specified by the <b>InterfaceLuid</b> or <b>InterfaceIndex</b> member of the <a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a> pointed to by the <i>Row</i> parameter could not be found.  

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_SUPPORTED</b></dt>
</dl>
</td>
<td width="60%">
The request is not supported. This error is returned if no IPv4 stack is on the local computer and an IPv4 address was specified in the <b>Address</b> member of the <a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a> pointed to by the <i>Row</i> parameter or no IPv6 stack is on the local computer and an IPv6 address was specified in the <b>Address</b> member.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>Other</b></dt>
</dl>
</td>
<td width="60%">
Use 
<a href="https://msdn.microsoft.com/b9d61342-4bcf-42e9-96f1-a5993dfb6c0c">FormatMessage</a> to obtain the message string for the returned error.

</td>
</tr>
</table>
 




## -remarks



The <b>ResolveIpNetEntry2</b> function is defined on Windows Vista and later. 

The <b>ResolveIpNetEntry2</b> function is used to resolve the physical address for a neighbor IP address entry on a local computer. This function flushes any existing neighbor entry that matches the IP address on the interface and then resolves the physical address (MAC) address
    by sending ARP requests for an IPv4 address or neighbor solicitation requests for an IPv6 address.
    If the <i>SourceAddress</i> parameter is specified, the <b>ResolveIpNetEntry2</b> function will select the
    interface with this source IP address to send the requests on.
If the <i>SourceAddress</i> parameter is not specified (NULL was passed in this parameter), the <b>ResolveIpNetEntry2</b> function will automatically select the
    best interface to send the requests on.


The <b>Address</b> member in the <a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a> structure pointed to by the <i>Row</i> parameter must be initialized to a valid IPv4 or IPv6 address and family. In addition, at least one of the following members in the <b>MIB_IPNET_ROW2</b> structure pointed to the <i>Row</i> parameter must be initialized to the interface: the <b>InterfaceLuid</b> or <b>InterfaceIndex</b>.

    The fields are used in the order listed above. So if the <b>InterfaceLuid</b> is specified, then this member is used to determine the interface on which to add the unicast IP address. If no value was set for the  <b>InterfaceLuid</b> member (the values of this member was set to zero), then the <b>InterfaceIndex</b> member is next used to determine the interface. 

If the IP address passed in the <b>Address</b> member of the <a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a> pointed to by the <i>Row</i> parameter is a duplicate of an existing neighbor IP address on the interface, the <b>ResolveIpNetEntry2</b> function will flush the existing entry before resolving the IP address. 

On output when the call is successful, <b>ResolveIpNetEntry2</b> retrieves the other properties for the neighbor IP address and fills out the <a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a> structure pointed to by the <i>Row</i> parameter. The  <b>PhysicalAddress</b> and <b>PhysicalAddressLength</b> members in the <b>MIB_IPNET_ROW2</b> structure pointed to by the <i>Row</i> parameter will be initialized to a valid physical address. 




## -see-also




<a href="https://msdn.microsoft.com/ca92b9f8-ec3c-4889-b649-f606c3920f92">CreateIpNetEntry2</a>



<a href="https://msdn.microsoft.com/85bace04-6c95-4cf2-a212-764de292aed6">DeleteIpNetEntry2</a>



<a href="https://msdn.microsoft.com/6ebfca41-acc3-450c-a3c5-881b8c3fca5e">FlushIpNetTable2</a>



<a href="https://msdn.microsoft.com/c77e01da-2d5a-4c74-b581-62fa6ee52c9e">GetIpNetEntry2</a>



<a href="https://msdn.microsoft.com/6c45d735-9a07-41ca-8d8a-919f32c98a3c">GetIpNetTable2</a>



<a href="https://msdn.microsoft.com/164dbd93-4464-40f9-989a-17597102b1d8">MIB_IPNET_ROW2</a>



<a href="https://msdn.microsoft.com/39b87d81-69ce-4f9b-8af6-5e0c5051657c">MIB_IPNET_TABLE2</a>



<a href="https://msdn.microsoft.com/7278dcb4-65c6-4aea-a474-cb7fae4d7672">SOCKADDR_INET</a>



<a href="https://msdn.microsoft.com/4f423700-f721-44a9-ade3-ea5b5b86e394">SetIpNetEntry2</a>
 

 

