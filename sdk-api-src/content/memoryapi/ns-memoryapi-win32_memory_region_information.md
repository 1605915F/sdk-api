---
UID: NS:memoryapi.WIN32_MEMORY_REGION_INFORMATION
title: WIN32_MEMORY_REGION_INFORMATION
author: windows-sdk-content
description: Contains information about a memory region.
old-location: base\win32_memory_region_information.htm
tech.root: memory
ms.assetid: C85C4B35-EED3-4BD4-A322-7C56BCB9D858
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WIN32_MEMORY_REGION_INFORMATION, WIN32_MEMORY_REGION_INFORMATION structure, base.win32_memory_region_information, memoryapi/WIN32_MEMORY_REGION_INFORMATION
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: memoryapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1607 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - MemoryApi.h
api_name:
 - WIN32_MEMORY_REGION_INFORMATION
product: Windows
targetos: Windows
req.typenames: WIN32_MEMORY_REGION_INFORMATION
req.redist: 
---

# WIN32_MEMORY_REGION_INFORMATION structure


## -description


Contains information about a memory region. A memory region is a single allocation that is created using a memory allocation function, such as <a href="https://msdn.microsoft.com/a720dd89-c47c-4e48-bbc6-f2e02dfc4ed2">VirtualAlloc</a> or <a href="https://msdn.microsoft.com/df9f54cd-b2de-4107-a1c5-d5a07045851e">MapViewOfFile</a>.


## -struct-fields




### -field AllocationBase

The base address of the allocation.


### -field AllocationProtect

The page protection value that was specified when the allocation was created. Protections of individual pages within the allocation can be different from this value. To query protection values of individual pages, use the <a href="https://msdn.microsoft.com/3b1f7d27-1f5d-452e-b58f-560cd9b9cbd3">VirtualQuery</a> function.


### -field DUMMYUNIONNAME

 


### -field DUMMYUNIONNAME.Flags

Represents all memory region flags as a single ULONG value. Applications should not use this field. Instead, test the individual bit field flags defined below.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME

 


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.Private

A value of 1 indicates that the allocation is private to the process. 


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.MappedDataFile

A value of 1 indicates that the allocation is a mapped view of a data file.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.MappedImage

A value of 1 indicates that the allocation is a mapped view of an executable image.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.MappedPageFile

A value of 1 indicates that the allocation is a mapped view of a pagefile-backed section.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.MappedPhysical

A value of 1 indicates that the allocation is a view of the <b>\Device\PhysicalMemory</b> section.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.DirectMapped

A value of 1 indicates that the allocation is a mapped view of a direct-mapped file.


### -field DUMMYUNIONNAME.DUMMYSTRUCTNAME.Reserved

Reserved.


### -field RegionSize

The size of the allocation.


### -field CommitSize

The commit charge associated with the allocation. For private allocations, this is the combined size of pages in the region that are committed, as opposed to reserved. For mapped views, this is the combined size of pages that have copy-on-write protection, or have been made private as a result of copy-on-write.


## -remarks



The <b>WIN32_MEMORY_REGION_INFORMATION</b> structure contains information about a single memory allocation. In contrast, the <a href="https://msdn.microsoft.com/dc3fa48e-0986-49cc-88a9-ff8179fbe5f0">MEMORY_BASIC_INFORMATION</a> structure that is returned by the <a href="https://msdn.microsoft.com/3b1f7d27-1f5d-452e-b58f-560cd9b9cbd3">VirtualQuery</a> function describes a contiguous run of pages within a single allocation that all have the same type, state, and protection. The mapping between <b>WIN32_MEMORY_REGION_INFORMATION</b> fields and memory type values returned by <b>VirtualQuery</b> is as follows:

<table>
<tr>
<th>WIN32_MEMORY_REGION_INFORMATION</th>
<th>MEMORY_BASIC_INFORMATION::Type</th>
</tr>
<tr>
<td>Private</td>
<td>MEM_PRIVATE</td>
</tr>
<tr>
<td>MappedDataFile</td>
<td>MEM_MAPPED</td>
</tr>
<tr>
<td>MappedImage</td>
<td>MEM_IMAGE</td>
</tr>
<tr>
<td>MappedPageFile</td>
<td>MEM_MAPPED</td>
</tr>
<tr>
<td>MappedPhysical</td>
<td>MEM_MAPPED</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/dc3fa48e-0986-49cc-88a9-ff8179fbe5f0">MEMORY_BASIC_INFORMATION</a>



<a href="https://msdn.microsoft.com/df9f54cd-b2de-4107-a1c5-d5a07045851e">MapViewOfFile</a>



<a href="https://msdn.microsoft.com/a720dd89-c47c-4e48-bbc6-f2e02dfc4ed2">VirtualAlloc</a>



<a href="https://msdn.microsoft.com/3b1f7d27-1f5d-452e-b58f-560cd9b9cbd3">VirtualQuery</a>
 

 

