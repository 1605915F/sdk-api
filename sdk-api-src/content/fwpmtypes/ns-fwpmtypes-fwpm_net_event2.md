---
UID: NS:fwpmtypes.FWPM_NET_EVENT2_
title: FWPM_NET_EVENT2 (fwpmtypes.h)
author: windows-sdk-content
description: Contains information about all event types.
old-location: fwp\fwpm_net_event2.htm
tech.root: fwp
ms.assetid: fbcacfb1-b471-474e-bdee-12a481fadc63
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FWPM_NET_EVENT2, FWPM_NET_EVENT2 structure [Filtering], fwp.fwpm_net_event2, fwpmtypes/FWPM_NET_EVENT2
ms.topic: struct
req.header: fwpmtypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - FWPM_NET_EVENT2
product: Windows
targetos: Windows
req.typenames: FWPM_NET_EVENT2
req.redist: 
ms.custom: 19H1
---

# FWPM_NET_EVENT2 structure


## -description


The <b>FWPM_NET_EVENT2</b> structure contains information about all event types.
<div class="alert"><b>Note</b>  <b>FWPM_NET_EVENT2</b> is the specific implementation of FWPM_NET_EVENT used in Windows 8. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 7, <a href="https://msdn.microsoft.com/0f989f66-8373-4546-ade3-8b337c4507e2">FWPM_NET_EVENT1</a> is available. For Windows Vista, <a href="https://msdn.microsoft.com/91e15135-49b8-497e-8f09-984e9af64dbe">FWPM_NET_EVENT0</a> is available.</div><div> </div>

## -struct-fields




### -field header

Type: <b><a href="https://msdn.microsoft.com/1120d807-9188-4674-9acd-4b96e680f8af">FWPM_NET_EVENT_HEADER2</a></b>

Information common to all events.


### -field type

Type: <b><a href="https://msdn.microsoft.com/75dd3b0f-d809-421e-ac70-b8bf5d38757c">FWPM_NET_EVENT_TYPE</a></b>

The type of event.


### -field ikeMmFailure

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Ee707313(v=VS.85).aspx">FWPM_NET_EVENT_IKEEXT_MM_FAILURE1</a>*</b>

Information about  an IKE main mode failure.

Available when <b>type</b> is <b>FWPM_NET_EVENT_TYPE_IKEEXT_MM_FAILURE</b>.


### -field ikeQmFailure

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa364280(v=VS.85).aspx">FWPM_NET_EVENT_IKEEXT_QM_FAILURE0</a>*</b>

Information about  an IKE quick mode failure.

Available when <b>type</b> is <b>FWPM_NET_EVENT_TYPE_IKEEXT_QM_FAILURE</b>.


### -field ikeEmFailure

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Ee707312(v=VS.85).aspx">FWPM_NET_EVENT_IKEEXT_EM_FAILURE1</a>*</b>

Information about  an IKE user mode failure.

Available when <b>type</b> is <b>FWPM_NET_EVENT_TYPE_IKEEXT_EM_FAILURE</b>.


### -field classifyDrop

Type: <b><a href="https://msdn.microsoft.com/1e018d6c-ed56-43f9-90b3-f2af42861617">FWPM_NET_EVENT_CLASSIFY_DROP2</a>*</b>

Information about  a drop event.

Available when <b>type</b> is <b>FWPM_NET_EVENT_TYPE_CLASSIFY_DROP</b>.


### -field ipsecDrop

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa814096(v=VS.85).aspx">FWPM_NET_EVENT_IPSEC_KERNEL_DROP0</a>*</b>

Information about an IPsec kernel drop event.

Available when <b>type</b> is <b>FWPM_NET_EVENT_TYPE_IPSEC_KERNEL_DROP</b>.


### -field idpDrop

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dd744950(v=VS.85).aspx">FWPM_NET_EVENT_IPSEC_DOSP_DROP0</a>*</b>

Information about an IPsec DoS Protection event.

Available when <b>type</b> is <b>FWPM_NET_EVENT_IPSEC_DOSP_DROP</b>.


### -field classifyAllow

Type: <b><a href="https://msdn.microsoft.com/4c7b665e-b248-4506-8d5f-bd27b05d8d50">FWPM_NET_EVENT_CLASSIFY_ALLOW0</a>*</b>

Information about an allow event.


### -field capabilityDrop

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh447364(v=VS.85).aspx">FWPM_NET_EVENT_CAPABILITY_DROP0</a>*</b>

Information about a capability-related drop event.


### -field capabilityAllow

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh447362(v=VS.85).aspx">FWPM_NET_EVENT_CAPABILITY_ALLOW0</a>*</b>

Information about a capability-related allow event.


### -field classifyDropMac

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh969202(v=VS.85).aspx">FWPM_NET_EVENT_CLASSIFY_DROP_MAC0</a>*</b>

Information about a MAC layer drop event.


## -see-also




<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 

