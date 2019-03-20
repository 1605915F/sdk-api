---
UID: NE:fwpstypes.FWPS_DISCARD_MODULE0_
title: FWPS_DISCARD_MODULE0 (fwpstypes.h)
author: windows-sdk-content
description: The FWPS_DISCARD_MODULE0 enumeration type specifies the type of module that discarded the data.Note  FWPS_DISCARD_MODULE0 is a specific version of FWPS_DISCARD_MODULE.
old-location: netvista\fwps_discard_module0.htm
tech.root: NetVista
ms.assetid: d9237268-a5e1-4b1c-91f7-9e894876ca87
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FWPS_DISCARD_MODULE0, FWPS_DISCARD_MODULE0 enumeration [Network Drivers Starting with Windows Vista], FWPS_DISCARD_MODULE_GENERAL, FWPS_DISCARD_MODULE_MAX, FWPS_DISCARD_MODULE_NETWORK, FWPS_DISCARD_MODULE_TRANSPORT, fwpstypes/FWPS_DISCARD_MODULE0, fwpstypes/FWPS_DISCARD_MODULE_GENERAL, fwpstypes/FWPS_DISCARD_MODULE_MAX, fwpstypes/FWPS_DISCARD_MODULE_NETWORK, fwpstypes/FWPS_DISCARD_MODULE_TRANSPORT, netvista.fwps_discard_module0, wfp_ref_4_enum_9cf37d53-bbf0-45ec-adc8-e690b4fd8aea.xml
ms.topic: enum
req.header: fwpstypes.h
req.include-header: Fwpsk.h
req.target-type: Windows
req.target-min-winverclnt: Supported starting with  Windows Vista.
req.target-min-winversvr: 
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
 - fwpstypes.h
api_name:
 - FWPS_DISCARD_MODULE0
product: Windows
targetos: Windows
req.typenames: FWPS_DISCARD_MODULE0
req.redist: 
---

# FWPS_DISCARD_MODULE0 enumeration


## -description


The <b>FWPS_DISCARD_MODULE0</b> enumeration type specifies the type of module that discarded the
  data.
<div class="alert"><b>Note</b>  <b>FWPS_DISCARD_MODULE0</b> is a specific version of <b>FWPS_DISCARD_MODULE</b>. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information.</div><div> </div>

## -enum-fields




### -field FWPS_DISCARD_MODULE_NETWORK

The data was discarded by the network layer.


### -field FWPS_DISCARD_MODULE_TRANSPORT

The data was discarded by the transport layer.


### -field FWPS_DISCARD_MODULE_GENERAL

The data was discarded by the filter engine.


### -field FWPS_DISCARD_MODULE_MAX

The maximum value for this enumeration. This value might change in future versions of the NDIS
     header files and binaries.


## -remarks



The 
    <a href="https://msdn.microsoft.com/f17076d8-b669-4bb4-a871-10c7bdc6e370">FWPS_DISCARD_METADATA0</a> structure
    contains a member of type FWPS_DISCARD_MODULE0 that specifies the type of module that discarded the
    data.




## -see-also




<a href="https://msdn.microsoft.com/f17076d8-b669-4bb4-a871-10c7bdc6e370">FWPS_DISCARD_METADATA0</a>
 

 

