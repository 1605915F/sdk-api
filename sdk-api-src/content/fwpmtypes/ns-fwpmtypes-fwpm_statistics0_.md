---
UID: NS:fwpmtypes.FWPM_STATISTICS0_
title: FWPM_STATISTICS0_
author: windows-sdk-content
description: Stores statistics related to connections at specific layers.
old-location: fwp\fwpm_statistics0.htm
tech.root: fwp
ms.assetid: c3ac6871-79b1-4378-8f3c-a56e85fd2a3b
ms.author: windowssdkdev
ms.date: 10/12/2018
ms.keywords: FWPM_STATISTICS0, FWPM_STATISTICS0 structure [Filtering], FWPM_STATISTICS0_, fwp.fwpm_statistics0, fwpmtypes/FWPM_STATISTICS0
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: fwpmtypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Fwpmtypes.idl
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
 - Fwpmtypes.h
api_name:
 - FWPM_STATISTICS0
product: Windows
targetos: Windows
req.typenames: FWPM_STATISTICS0
req.redist: 
---

# FWPM_STATISTICS0_ structure


## -description


The <b>FWPM_STATISTICS0</b> structure stores statistics related to connections at specific layers.


## -struct-fields




### -field numLayerStatistics

Type: <b>UINT32</b>

Number of <a href="https://msdn.microsoft.com/cc8e0159-fe28-4718-b5fe-d38d180b3e2c">FWPM_LAYER_STATISTICS0</a> structures in the <b>layerStatistics</b> member.


### -field layerStatistics

Type: <b><a href="https://msdn.microsoft.com/cc8e0159-fe28-4718-b5fe-d38d180b3e2c">FWPM_LAYER_STATISTICS0</a>*</b>

Statistics related to the layer.


### -field inboundAllowedConnectionsV4

Type: <b>UINT32</b>

Number of allowed IPv4 inbound connections.


### -field inboundBlockedConnectionsV4

Type: <b>UINT32</b>

Number of blocked IPv4 inbound connections.


### -field outboundAllowedConnectionsV4

Type: <b>UINT32</b>

Number of allowed IPv4 outbound connections.


### -field outboundBlockedConnectionsV4

Type: <b>UINT32</b>

Number of blocked IPv4 outbound connections.


### -field inboundAllowedConnectionsV6

Type: <b>UINT32</b>

Number of allowed IPv6 inbound connections.


### -field inboundBlockedConnectionsV6

Type: <b>UINT32</b>

Number of blocked IPv6 inbound connections.


### -field outboundAllowedConnectionsV6

Type: <b>UINT32</b>

Number of allowed IPv6 outbound connections.


### -field outboundBlockedConnectionsV6

Type: <b>UINT32</b>

Number of blocked IPv6 outbound connections.


### -field inboundActiveConnectionsV4

Type: <b>UINT32</b>

Number of active IPv4 inbound connections.


### -field outboundActiveConnectionsV4

Type: <b>UINT32</b>

Number of active IPv4 outbound connections.


### -field inboundActiveConnectionsV6

Type: <b>UINT32</b>

Number of active IPv6 inbound connections.


### -field outboundActiveConnectionsV6

Type: <b>UINT32</b>

Number of active IPv6 outbound connections.


### -field reauthDirInbound

 


### -field reauthDirOutbound

 


### -field reauthFamilyV4

 


### -field reauthFamilyV6

 


### -field reauthProtoOther

 


### -field reauthProtoIPv4

 


### -field reauthProtoIPv6

 


### -field reauthProtoICMP

 


### -field reauthProtoICMP6

 


### -field reauthProtoUDP

 


### -field reauthProtoTCP

 


### -field reauthReasonPolicyChange

 


### -field reauthReasonNewArrivalInterface

 


### -field reauthReasonNewNextHopInterface

 


### -field reauthReasonProfileCrossing

 


### -field reauthReasonClassifyCompletion

 


### -field reauthReasonIPSecPropertiesChanged

 


### -field reauthReasonMidStreamInspection

 


### -field reauthReasonSocketPropertyChanged

 


### -field reauthReasonNewInboundMCastBCastPacket

 


### -field reauthReasonEDPPolicyChanged

 


### -field reauthReasonPreclassifyLocalAddrLayerChange

 


### -field reauthReasonPreclassifyRemoteAddrLayerChange

 


### -field reauthReasonPreclassifyLocalPortLayerChange

 


### -field reauthReasonPreclassifyRemotePortLayerChange

 


### -field reauthReasonProxyHandleChanged

 




## -remarks



<b>FWPM_STATISTICS0</b> is a specific implementation of FWPM_STATISTICS. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a>  for more information.




## -see-also




<a href="https://msdn.microsoft.com/cc8e0159-fe28-4718-b5fe-d38d180b3e2c">FWPM_LAYER_STATISTICS0</a>
 

 

