---
UID: NF:dxgidebug.IDXGIInfoQueue.PushCopyOfStorageFilter
title: IDXGIInfoQueue::PushCopyOfStorageFilter
author: windows-sdk-content
description: Pushes a copy of the storage filter that is currently on the top of the storage-filter stack onto the storage-filter stack.
old-location: direct3ddxgi\idxgiinfoqueue_pushcopyofstoragefilter.htm
tech.root: direct3ddxgi
ms.assetid: 1CD32898-90B1-4523-8C97-985CA9F7D92B
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDXGIInfoQueue interface [DXGI],PushCopyOfStorageFilter method, IDXGIInfoQueue.PushCopyOfStorageFilter, IDXGIInfoQueue::PushCopyOfStorageFilter, PushCopyOfStorageFilter, PushCopyOfStorageFilter method [DXGI], PushCopyOfStorageFilter method [DXGI],IDXGIInfoQueue interface, direct3ddxgi.idxgiinfoqueue_pushcopyofstoragefilter, dxgidebug/IDXGIInfoQueue::PushCopyOfStorageFilter
ms.topic: method
req.header: dxgidebug.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
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
req.dll: DXGIDebug.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - DXGIDebug.dll
api_name:
 - IDXGIInfoQueue.PushCopyOfStorageFilter
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIInfoQueue::PushCopyOfStorageFilter


## -description


Pushes a copy of the storage filter that is currently on the top of the storage-filter stack onto the storage-filter stack.


## -parameters




### -param Producer [in]

 A <a href="https://msdn.microsoft.com/85946D30-5E49-4E4B-AC25-394ABFF0DB11">DXGI_DEBUG_ID</a> value that identifies the entity that pushes the copy of the storage filter.


## -returns



Returns S_OK if successful; an error code otherwise. For a list of error codes, see <a href="https://msdn.microsoft.com/en-us/library/Bb509553(v=VS.85).aspx">DXGI_ERROR</a>.




## -remarks



<div class="alert"><b>Note</b>  This API requires the Windows Software Development Kit (SDK) for Windows 8.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/F1BC6752-F334-4E8C-BE42-B731635A799D">IDXGIInfoQueue</a>
 

 

