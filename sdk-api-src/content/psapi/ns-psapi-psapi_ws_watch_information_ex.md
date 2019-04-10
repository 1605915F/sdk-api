---
UID: NS:psapi._PSAPI_WS_WATCH_INFORMATION_EX
title: PSAPI_WS_WATCH_INFORMATION_EX (psapi.h)
author: windows-sdk-content
description: Contains extended information about a page added to a process working set.
old-location: psapi\psapi_ws_watch_information_ex.htm
tech.root: psapi
ms.assetid: fb0429b1-ec93-401c-aeb1-f7e9d9acfa47
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PPSAPI_WS_WATCH_INFORMATION_EX, PPSAPI_WS_WATCH_INFORMATION_EX, PPSAPI_WS_WATCH_INFORMATION_EX structure pointer [PSAPI], PSAPI_WS_WATCH_INFORMATION_EX, PSAPI_WS_WATCH_INFORMATION_EX structure [PSAPI], base.psapi_ws_watch_information_ex, psapi.psapi_ws_watch_information_ex, psapi/PPSAPI_WS_WATCH_INFORMATION_EX, psapi/PSAPI_WS_WATCH_INFORMATION_EX"
ms.topic: struct
req.header: psapi.h
req.include-header: 
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
 - PSAPI_WS_WATCH_INFORMATION_EX
product: Windows
targetos: Windows
req.typenames: PSAPI_WS_WATCH_INFORMATION_EX, *PPSAPI_WS_WATCH_INFORMATION_EX
req.redist: 
---

# PSAPI_WS_WATCH_INFORMATION_EX structure


## -description


Contains extended information about a page added to a process working set.


## -struct-fields




### -field BasicInfo

A <a href="https://msdn.microsoft.com/61083366-2a55-431c-807a-3eb85ba0b347">PSAPI_WS_WATCH_INFORMATION</a> structure.


### -field FaultingThreadId

The identifier of the thread that caused the page fault.


### -field Flags

This member is reserved for future use.


## -see-also




<a href="https://msdn.microsoft.com/8572db5c-2ffc-424f-8cec-b6a6902fed62">GetWsChangesEx</a>



<a href="https://msdn.microsoft.com/61083366-2a55-431c-807a-3eb85ba0b347">PSAPI_WS_WATCH_INFORMATION</a>
 

 

