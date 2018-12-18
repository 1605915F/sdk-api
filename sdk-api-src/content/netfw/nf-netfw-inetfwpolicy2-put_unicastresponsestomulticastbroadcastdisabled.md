---
UID: NF:netfw.INetFwPolicy2.put_UnicastResponsesToMulticastBroadcastDisabled
title: INetFwPolicy2::put_UnicastResponsesToMulticastBroadcastDisabled
author: windows-sdk-content
description: Indicates whether the firewall should not allow unicast responses to multicast and broadcast traffic.
old-location: ics\inetfwpolicy2_unicastresponsestomulticastbroadcastdisabled.htm
tech.root: ics
ms.assetid: 4ab9cadf-7ecb-4b3d-a166-b491d89101d7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: INetFwPolicy2 interface [ICS/ICF],UnicastResponsesToMulticastBroadcastDisabled property, INetFwPolicy2.UnicastResponsesToMulticastBroadcastDisabled, INetFwPolicy2.put_UnicastResponsesToMulticastBroadcastDisabled, INetFwPolicy2::UnicastResponsesToMulticastBroadcastDisabled, INetFwPolicy2::get_UnicastResponsesToMulticastBroadcastDisabled, INetFwPolicy2::put_UnicastResponsesToMulticastBroadcastDisabled, UnicastResponsesToMulticastBroadcastDisabled property [ICS/ICF], UnicastResponsesToMulticastBroadcastDisabled property [ICS/ICF],INetFwPolicy2 interface, ics.inetfwpolicy2_unicastresponsestomulticastbroadcastdisabled, netfw/INetFwPolicy2::UnicastResponsesToMulticastBroadcastDisabled, netfw/INetFwPolicy2::get_UnicastResponsesToMulticastBroadcastDisabled, netfw/INetFwPolicy2::put_UnicastResponsesToMulticastBroadcastDisabled, put_UnicastResponsesToMulticastBroadcastDisabled
ms.topic: method
req.header: netfw.h
req.include-header: FirewallAPI.h, Netfw.h
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
req.lib: 
req.dll: Wfapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wfapi.dll
api_name:
 - INetFwPolicy2.UnicastResponsesToMulticastBroadcastDisabled
 - INetFwPolicy2.get_UnicastResponsesToMulticastBroadcastDisabled
 - INetFwPolicy2.put_UnicastResponsesToMulticastBroadcastDisabled
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# INetFwPolicy2::put_UnicastResponsesToMulticastBroadcastDisabled


## -description


Indicates whether the firewall should not allow unicast responses to multicast and
   broadcast traffic.

This property is read/write.


## -parameters


## -remarks



If a computer sends a broadcast packet, a unicast response is allowed for three seconds. Use this property to change this behavior.

When you pass a profile type obtained from the <a href="https://msdn.microsoft.com/93f4b508-30db-45a9-a7aa-df4a993dc50b">CurrentProfileTypes</a> property (<b>get_CurrentProfileTypes</b>), make sure that you pass only one profile type to <b>get_UnicastResponsesToMulticastBroadcastDisabled</b> and <b>put_UnicastResponsesToMulticastBroadcastDisabled</b>. Note that <b>get_CurrentProfileTypes</b> can return multiple profiles.




## -see-also




<a href="https://msdn.microsoft.com/ef01a531-ddb0-4eb4-894b-82f613016396">INetFwPolicy2</a>
 

 

