---
UID: NF:dhcpsapi.DhcpV4FailoverDeleteRelationship
title: DhcpV4FailoverDeleteRelationship function
author: windows-sdk-content
description: Deletes a DHCPv4 failover relationship between two servers.
old-location: dhcp\dhcpv4failoverdeleterelationship.htm
tech.root: DHCP
ms.assetid: c7b894a4-4def-41fe-98b6-f56d6ff0c715
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DhcpV4FailoverDeleteRelationship, DhcpV4FailoverDeleteRelationship function [DHCP], dhcp.dhcpv4failoverdeleterelationship, dhcpsapi/DhcpV4FailoverDeleteRelationship
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: dhcpsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dhcpsapi.lib
req.dll: Dhcpsapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Dhcpsapi.dll
api_name:
 - DhcpV4FailoverDeleteRelationship
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DhcpV4FailoverDeleteRelationship function


## -description


The <b>DhcpV4FailoverDeleteRelationship</b> function deletes a DHCPv4 failover relationship between two servers.


## -parameters




### -param ServerIpAddress [in, optional]

Pointer to a null-terminated Unicode string that represents the IP address or hostname of the DHCP server.


### -param pRelationshipName [in]

Pointer to null-terminated Unicode string that represents the name of the relationship to delete.


## -returns



If the function succeeds, it returns <b>ERROR_SUCCESS</b>.

If the function fails, it returns one of the following or an error code from <a href="https://msdn.microsoft.com/6370313f-d7db-4ff1-b0e0-7fa47474facb">DHCP Server Management API Error Codes</a>.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One or more of the parameters were invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_DHCP_FO_RELATIONSHIP_DOES_NOT_EXIST</b></dt>
</dl>
</td>
<td width="60%">
The failover relationship doesn't exist.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/6e360dd4-b4a0-4652-8754-17c3c284271c">DhcpV4FailoverCreateRelationship</a>



<a href="https://msdn.microsoft.com/81ef2af8-c1a9-44e7-857c-1591947609ed">DhcpV4FailoverEnumRelationship</a>



<a href="https://msdn.microsoft.com/b637d1e8-8c61-4382-a5ec-3d5395433f86">DhcpV4FailoverGetRelationship</a>



<a href="https://msdn.microsoft.com/04012953-dca3-426f-99de-798870d1eb97">DhcpV4FailoverSetRelationship</a>
 

 

