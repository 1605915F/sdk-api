---
UID: NS:dhcpsapi._DHCP_IP_RESERVATION_V6
title: DHCP_IP_RESERVATION_V6 (dhcpsapi.h)
author: windows-sdk-content
description: Defines an IPv6 reservation for a DHCPv6 client in a specific IPv6 prefix.
old-location: dhcp\dhcp_ip_reservation_v6.htm
tech.root: DHCP
ms.assetid: f1595632-018b-4626-b3c6-49f0e5b3752c
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*LPDHCP_IP_RESERVATION_V6, DHCP_IP_RESERVATION_V6, DHCP_IP_RESERVATION_V6 structure [DHCP], PDHCP_IP_RESERVATION_V6, PDHCP_IP_RESERVATION_V6 structure pointer [DHCP], dhcp.dhcp_ip_reservation_v6, dhcpsapi/DHCP_IP_RESERVATION_V6, dhcpsapi/PDHCP_IP_RESERVATION_V6"
ms.topic: struct
req.header: dhcpsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - Dhcpsapi.h
api_name:
 - DHCP_IP_RESERVATION_V6
product: Windows
targetos: Windows
req.typenames: DHCP_IP_RESERVATION_V6, *LPDHCP_IP_RESERVATION_V6
req.redist: 
ms.custom: 19H1
---

# DHCP_IP_RESERVATION_V6 structure


## -description


The <b>DHCP_IP_RESERVATION_V6</b> structure defines an IPv6 reservation for a DHCPv6 client in a specific IPv6 prefix. 


## -struct-fields




### -field ReservedIpAddress


<a href="https://msdn.microsoft.com/9623e866-81e5-4d5a-8801-33f0f8973ed3">DHCP_IPV6_ADDRESS</a> structure that contains the IPv6 address of the DHCPv6 client for which an IPv6 reservation is created.


### -field ReservedForClient


<a href="https://msdn.microsoft.com/0afdddb4-12f9-4c0b-937a-2cc311c126b4">DHCP_CLIENT_UID</a> structure that contains the hardware address (MAC address) of the DHCPv6 client for which the IPv6 reservation is created.


### -field InterfaceId

Integer that specifies the interface identifier for which the IPv6 reservation is created.


## -see-also




<a href="https://msdn.microsoft.com/9623e866-81e5-4d5a-8801-33f0f8973ed3">DHCP_IPV6_ADDRESS</a>



<a href="https://msdn.microsoft.com/4f0110b5-3770-4aae-8df7-d2481eac3417">DHCP_IP_RESERVATION_INFO</a>



<a href="https://msdn.microsoft.com/01951b18-fc54-4a34-9ccd-fd98f4e7864f">DHCP_IP_RESERVATION_V4</a>



<a href="https://msdn.microsoft.com/de5fa8c5-5cd7-4358-bacd-f27f4b7f3761">DHCP_SUBNET_ELEMENT_DATA_V6</a>
 

 

