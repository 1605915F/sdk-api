---
UID: NS:sensapi.tagQOCINFO
title: tagQOCINFO
author: windows-sdk-content
description: The QOCINFO structure is returned by the IsDestinationReachable function and provides Quality of Connection information to the caller.
old-location: sens\qocinfo.htm
tech.root: Sens
ms.assetid: 1f78a7c5-b3c7-4f21-8848-58cfb481f4bb
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: "*LPQOCINFO, LPQOCINFO, LPQOCINFO structure pointer [SENS], NETWORK_ALIVE_AOL, NETWORK_ALIVE_LAN, NETWORK_ALIVE_WAN, QOCINFO, QOCINFO structure [SENS], _zaw_qocinfo, sens.qocinfo, sensapi/LPQOCINFO, sensapi/QOCINFO, syncmgr.qocinfo, tagQOCINFO"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: sensapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - Sensapi.h
api_name:
 - QOCINFO
product: Windows
targetos: Windows
req.typenames: QOCINFO, *LPQOCINFO
req.redist: 
---

# tagQOCINFO structure


## -description


The 
<b>QOCINFO</b> structure is returned by the 
<a href="https://msdn.microsoft.com/377af331-8494-4a3d-b822-78c2b568239c">IsDestinationReachable</a> function and provides Quality of Connection information to the caller.


## -struct-fields




### -field dwSize

Upon calling 
<a href="https://msdn.microsoft.com/377af331-8494-4a3d-b822-78c2b568239c">IsDestinationReachable</a>, the caller must specify the size of the <b>QOCINFO</b> structure being provided to the function using dwSize. The size should be specified in bytes. Upon return from <a href="https://msdn.microsoft.com/377af331-8494-4a3d-b822-78c2b568239c">IsDestinationReachable</a>, dwSize contains the size of the provided structure in bytes.


### -field dwFlags

Provides information on the type of network connection available. The following table lists the possible values.

<table>
<tr>
<th>Flag</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="NETWORK_ALIVE_LAN"></a><a id="network_alive_lan"></a><dl>
<dt><b>NETWORK_ALIVE_LAN</b></dt>
<dt>0x00000001</dt>
</dl>
</td>
<td width="60%">
The computer has one or more active LAN cards.

</td>
</tr>
<tr>
<td width="40%"><a id="NETWORK_ALIVE_WAN"></a><a id="network_alive_wan"></a><dl>
<dt><b>NETWORK_ALIVE_WAN</b></dt>
<dt>0x00000002</dt>
</dl>
</td>
<td width="60%">
The computer has one or more active RAS connections.

</td>
</tr>
<tr>
<td width="40%"><a id="NETWORK_ALIVE_AOL"></a><a id="network_alive_aol"></a><dl>
<dt><b>NETWORK_ALIVE_AOL</b></dt>
<dt>0x00000004</dt>
</dl>
</td>
<td width="60%">
This flag is not supported.

</td>
</tr>
</table>
 


### -field dwInSpeed

Speed of data coming in from the destination in bytes per second.


### -field dwOutSpeed

Speed of data sent to the destination in bytes per second.


## -see-also




<a href="https://msdn.microsoft.com/377af331-8494-4a3d-b822-78c2b568239c">IsDestinationReachable</a>
 

 

