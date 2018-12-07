---
UID: NF:wsdutil.WSDFreeLinkedMemory
title: WSDFreeLinkedMemory function
author: windows-sdk-content
description: Frees a memory block previously allocated with WSDAllocateLinkedMemory.
old-location: ncd\wsdfreelinkedmemory_func.htm
tech.root: wsdapi
ms.assetid: 8fe6f586-a262-4248-9650-dec0fae8cd74
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WSDFreeLinkedMemory, WSDFreeLinkedMemory function, ncd.wsdfreelinkedmemory_func, wsdutil/WSDFreeLinkedMemory
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: wsdutil.h
req.include-header: Wsdapi.h
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
req.lib: Wsdapi.lib
req.dll: Wsdapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Wsdapi.dll
api_name:
 - WSDFreeLinkedMemory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WSDFreeLinkedMemory function


## -description


Frees a memory block previously allocated with <a href="https://msdn.microsoft.com/2608985f-56aa-4223-b76d-85ebe3b080fb">WSDAllocateLinkedMemory</a>.


## -parameters




### -param pVoid

Pointer to the memory block to be freed.


## -returns



This function does not return a value.




## -remarks



All children of the memory block are automatically freed.



