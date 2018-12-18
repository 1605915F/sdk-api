---
UID: NF:rtworkq.IRtwqAsyncResult.GetStateNoAddRef
title: IRtwqAsyncResult::GetStateNoAddRef
author: windows-sdk-content
description: Returns the state object specified by the caller in the asynchronous Begin method, without incrementing the object's reference count.
old-location: base\irtwqasyncresult_getstatenoaddref.htm
tech.root: procthread
ms.assetid: DF41E4E7-015C-469A-A94F-16F06445B804
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetStateNoAddRef, GetStateNoAddRef method, GetStateNoAddRef method,IRtwqAsyncResult interface, IRtwqAsyncResult interface,GetStateNoAddRef method, IRtwqAsyncResult.GetStateNoAddRef, IRtwqAsyncResult::GetStateNoAddRef, base.irtwqasyncresult_getstatenoaddref, rtworkq/IRtwqAsyncResult::GetStateNoAddRef
ms.topic: method
req.header: rtworkq.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Rtworkq.lib
req.dll: RTWorkQ.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - RTWorkQ.dll
api_name:
 - IRtwqAsyncResult.GetStateNoAddRef
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IRtwqAsyncResult::GetStateNoAddRef


## -description



Returns the state object specified by the caller in the asynchronous <b>Begin</b> method, without incrementing the object's reference count.




## -parameters






## -returns



Returns a pointer to the state object's <b>IUnknown</b> interface, or <b>NULL</b> if no object was set. This pointer does not have an outstanding reference count. If you store this pointer, you must call <b>AddRef</b> on the pointer.




## -see-also




<a href="https://msdn.microsoft.com/AB23282D-D731-48EE-AF55-CC5A513EBA33">IRtwqAsyncResult</a>
 

 

