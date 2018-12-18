---
UID: NN:rdpencomapi.IRDPSRAPIAttendeeManager
title: IRDPSRAPIAttendeeManager
author: windows-sdk-content
description: Manages attendee objects.
old-location: rdp\irdpsrapiattendeemanager.htm
tech.root: rdp
ms.assetid: 202b539c-b7a0-4cf3-ba64-f60cc062575a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IRDPSRAPIAttendeeManager, IRDPSRAPIAttendeeManager interface [RDP], IRDPSRAPIAttendeeManager interface [RDP],described, rdp.irdpsrapiattendeemanager, rdpencomapi/IRDPSRAPIAttendeeManager
ms.topic: interface
req.header: rdpencomapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: RdpEncomAPI.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: RdpEncomAPI.tlb
req.lib: 
req.dll: RdpEncom.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - RdpEncom.dll
api_name:
 - IRDPSRAPIAttendeeManager
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRDPSRAPIAttendeeManager interface


## -description


Manages attendee objects.

Applications obtain access to this object using <a href="https://msdn.microsoft.com/bcbc8f16-855d-4835-966c-73773f3ac6d4">IRDPSRAPISharingSession::get_Attendees</a>.


## -remarks



The lifetime of the objects in this collection is controlled by the network layer.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms221608(v=VS.85).aspx">IDispatch</a>



<a href="https://msdn.microsoft.com/e9edd9f2-ccbf-45b2-b71c-e30368435a60">IRDPSRAPIAttendee</a>
 

 

