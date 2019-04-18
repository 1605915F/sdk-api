---
UID: NS:psapi._PROCESS_MEMORY_COUNTERS
title: PROCESS_MEMORY_COUNTERS (psapi.h)
author: windows-sdk-content
description: Contains the memory statistics for a process.
old-location: psapi\process_memory_counters_str.htm
tech.root: psapi
ms.assetid: 288b5865-28a3-478b-ad32-c710fe4f3a81
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PPROCESS_MEMORY_COUNTERS, PPROCESS_MEMORY_COUNTERS, PPROCESS_MEMORY_COUNTERS structure pointer [PSAPI], PROCESS_MEMORY_COUNTERS, PROCESS_MEMORY_COUNTERS structure [PSAPI], _win32_process_memory_counters_str, base.process_memory_counters_str, psapi.process_memory_counters_str, psapi/PPROCESS_MEMORY_COUNTERS, psapi/PROCESS_MEMORY_COUNTERS"
ms.topic: struct
req.header: psapi.h
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
 - Psapi.h
api_name:
 - PROCESS_MEMORY_COUNTERS
product: Windows
targetos: Windows
req.typenames: PROCESS_MEMORY_COUNTERS
req.redist: 
ms.custom: 19H1
---

# PROCESS_MEMORY_COUNTERS structure


## -description


Contains the memory statistics for a process.


## -struct-fields




### -field cb

The size of the structure, in bytes.


### -field PageFaultCount

The number of page faults.


### -field PeakWorkingSetSize

The peak working set size, in bytes.


### -field WorkingSetSize

The current working set size, in bytes.


### -field QuotaPeakPagedPoolUsage

The peak paged pool usage, in bytes.


### -field QuotaPagedPoolUsage

The current paged pool usage, in bytes.


### -field QuotaPeakNonPagedPoolUsage

The peak nonpaged pool usage, in bytes.


### -field QuotaNonPagedPoolUsage

The current nonpaged pool usage, in bytes.


### -field PagefileUsage

The Commit Charge value in bytes for this process. Commit Charge is the total amount of memory that the memory manager has committed for a running process.


### -field PeakPagefileUsage

The peak value in bytes of the Commit Charge during the lifetime of this process.


## -see-also




<a href="https://msdn.microsoft.com/12990e8d-6097-4502-824e-db6c3f76c715">GetProcessMemoryInfo</a>



<a href="https://msdn.microsoft.com/b27ca747-8fd2-4267-9979-4e2e14a5a19f">Memory Performance Information</a>



<a href="https://msdn.microsoft.com/683c899e-a7e8-4440-8f13-2a713c1618bf">Process Memory Usage Information</a>



<a href="https://msdn.microsoft.com/33c42f79-cc77-4d44-84c3-8bf0a4a60019">Working Set Information</a>
 

 

