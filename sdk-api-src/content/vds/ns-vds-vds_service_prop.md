---
UID: NS:vds._VDS_SERVICE_PROP
title: VDS_SERVICE_PROP
author: windows-sdk-content
description: Defines the properties of the service object.
old-location: base\vds_service_prop.htm
tech.root: VDS
ms.assetid: 9029ebbd-f05d-4317-913d-58c8a0a62886
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: VDS_SERVICE_PROP, VDS_SERVICE_PROP structure [VDS], base.vds_service_prop, vds/_VDS_SERVICE_PROP
ms.topic: struct
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
 - Vds.h
api_name:
 - VDS_SERVICE_PROP
product: Windows
targetos: Windows
req.typenames: VDS_SERVICE_PROP
req.redist: 
---

# VDS_SERVICE_PROP structure


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Defines the properties of the <a href="https://msdn.microsoft.com/ae4d18f2-4d50-480c-bc7a-4eec0334707d">service object</a>.


## -struct-fields




### -field pwszVersion

The version of VDS; a zero-terminated, human-readable string.


### -field ulFlags

A bitmask of <a href="https://msdn.microsoft.com/d14718bd-43a3-4775-a218-27c59f6995eb">VDS_SERVICE_FLAG</a> enumeration values that describe the service.


## -remarks



 The <a href="https://msdn.microsoft.com/fb5fe743-4833-400a-a8aa-8de886203190">IVdsService::GetProperties</a>method returns this structure to report the properties of the <a href="https://msdn.microsoft.com/ae4d18f2-4d50-480c-bc7a-4eec0334707d">service object</a>.




## -see-also




<a href="https://msdn.microsoft.com/fb5fe743-4833-400a-a8aa-8de886203190">IVdsService::GetProperties</a>



<a href="https://msdn.microsoft.com/6a13f5eb-0fa1-48e2-a112-b2254ca28423">VDS Structures</a>
 

 

