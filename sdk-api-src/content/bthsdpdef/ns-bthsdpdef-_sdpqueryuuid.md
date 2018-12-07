---
UID: NS:bthsdpdef._SdpQueryUuid
title: "_SdpQueryUuid"
author: windows-sdk-content
description: The SdpQueryUuid structure facilitates searching for UUIDs.
old-location: bluetooth\sdpqueryuuid.htm
tech.root: Bluetooth
ms.assetid: 8c67b1b1-d289-4273-a512-589b19cd1f85
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: SdpQueryUuid, SdpQueryUuid structure [Bluetooth], _SdpQueryUuid, bluetooth.sdpqueryuuid, bthsdpdef/SdpQueryUuid
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: bthsdpdef.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Bthsdpdef.h
api_name:
 - SdpQueryUuid
product: Windows
targetos: Windows
req.typenames: SdpQueryUuid
req.redist: 
---

# _SdpQueryUuid structure


## -description


The <b>SdpQueryUuid</b> structure facilitates searching for UUIDs.


## -struct-fields




### -field u

Union containing the UUID on which to search.


### -field u.switch_is

 


### -field u.switch_is.uuidType

 


### -field uuidType

Type of UUID being searched. Must be one of the three valid values from the SDP_SPECIFICTYPE enumeration:


<ul>
<li>SDP_ST_UUID16 - indicates u.uuid16 will be used in the search.</li>
<li>SDP_ST_UUID32 - indicates u.uuid32 will be used in the search.</li>
<li>SDP_ST_UUID128 - indicates u.uuid128 will be used in the search.</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa362938(v=VS.85).aspx">BTH_QUERY_SERVICE</a>
 

 

