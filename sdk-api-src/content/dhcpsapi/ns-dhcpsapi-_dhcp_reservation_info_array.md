---
UID: NS:dhcpsapi._DHCP_RESERVATION_INFO_ARRAY
title: "_DHCP_RESERVATION_INFO_ARRAY"
author: windows-sdk-content
description: The DHCP_RESERVATION_INFO_ARRAY structure defines an array of IPv4 reservations for DHCPv4 clients.
old-location: dhcp\dhcp_reservation_info_array.htm
tech.root: DHCP
ms.assetid: 9823ee47-6b61-4256-8fac-d301d72774ec
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPDHCP_RESERVATION_INFO_ARRAY, DHCP_RESERVATION_INFO_ARRAY, DHCP_RESERVATION_INFO_ARRAY structure [DHCP], LPDHCP_RESERVATION_INFO_ARRAY, LPDHCP_RESERVATION_INFO_ARRAY structure pointer [DHCP], _DHCP_RESERVATION_INFO_ARRAY, dhcp.dhcp_reservation_info_array, dhcpsapi/DHCP_RESERVATION_INFO_ARRAY, dhcpsapi/LPDHCP_RESERVATION_INFO_ARRAY"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - dhcpsapi.h
api_name:
 - DHCP_RESERVATION_INFO_ARRAY
product: Windows
targetos: Windows
req.typenames: DHCP_RESERVATION_INFO_ARRAY, *LPDHCP_RESERVATION_INFO_ARRAY
req.redist: 
---

# _DHCP_RESERVATION_INFO_ARRAY structure


## -description


The <b>DHCP_RESERVATION_INFO_ARRAY</b> structure defines an array of IPv4 reservations for DHCPv4 clients.


## -struct-fields




### -field NumElements

Integer that specifies the number of IPv4 client reservations in <b>Elements</b>.


### -field Elements

Pointer to an array of <a href="https://msdn.microsoft.com/4f0110b5-3770-4aae-8df7-d2481eac3417">DHCP_IP_RESERVATION_INFO</a> structures that contain IPv4 client reservations.


### -field Elements.size_is

 


### -field Elements.size_is.NumElements

 




## -see-also




<a href="https://msdn.microsoft.com/6eebc858-7ffe-4bf3-b318-3a5ad16c9827">DhcpV4EnumSubnetReservations</a>
 

 

