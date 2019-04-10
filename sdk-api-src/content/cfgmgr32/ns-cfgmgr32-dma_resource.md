---
UID: NS:cfgmgr32.DMA_Resource_s
title: DMA_RESOURCE (cfgmgr32.h)
author: windows-sdk-content
description: The DMA_RESOURCE structure is used for specifying either a resource list or a resource requirements list that describes DMA channel usage for a device instance.
old-location: devinst\dma_resource.htm
tech.root: devinst
ms.assetid: 226a5ca1-10e1-47a7-8bd9-b153a0784ccb
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PDMA_RESOURCE, DMA_RESOURCE, DMA_RESOURCE structure [Device and Driver Installation], PDMA_RESOURCE, PDMA_RESOURCE structure pointer [Device and Driver Installation], cfgmgr32/DMA_RESOURCE, cfgmgr32/PDMA_RESOURCE, cfgmgrst_7efdb1b3-3104-4bbe-81a6-e118a75a70a3.xml, devinst.dma_resource"
ms.topic: struct
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Windows
req.target-min-winverclnt: 
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
 - cfgmgr32.h
api_name:
 - DMA_RESOURCE
product: Windows
targetos: Windows
req.typenames: DMA_RESOURCE, *PDMA_RESOURCE
req.redist: 
---

# DMA_RESOURCE structure


## -description


The DMA_RESOURCE structure is used for specifying either a resource list or a resource requirements list that describes DMA channel usage for a device instance. For more information about resource list and resource requirements lists, see <a href="https://msdn.microsoft.com/c7a6997b-34f9-4dd9-b384-2321a8b5ce54">Hardware Resources</a>.


## -struct-fields




### -field DMA_Header

A <a href="https://msdn.microsoft.com/e357132d-ba40-4c14-813c-505aadc94a26">DMA_DES</a> structure.


### -field DMA_Data





#### For a resource list:

Zero.



#### For a resource requirements list:

A <a href="https://msdn.microsoft.com/46c80013-1863-4e02-be8d-282d2e619200">DMA_RANGE</a> array.


## -see-also




<a href="https://msdn.microsoft.com/e357132d-ba40-4c14-813c-505aadc94a26">DMA_DES</a>



<a href="https://msdn.microsoft.com/46c80013-1863-4e02-be8d-282d2e619200">DMA_RANGE</a>
 

 

