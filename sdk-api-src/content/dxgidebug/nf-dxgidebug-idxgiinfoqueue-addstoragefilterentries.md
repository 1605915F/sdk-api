---
UID: NF:dxgidebug.IDXGIInfoQueue.AddStorageFilterEntries
title: IDXGIInfoQueue::AddStorageFilterEntries (dxgidebug.h)
author: windows-sdk-content
description: Adds storage filters to the top of the storage-filter stack.
old-location: direct3ddxgi\idxgiinfoqueue_addstoragefilterentries.htm
tech.root: direct3ddxgi
ms.assetid: 34FC5AE3-7B72-4480-ACFA-53C7FB5425DA
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: AddStorageFilterEntries, AddStorageFilterEntries method [DXGI], AddStorageFilterEntries method [DXGI],IDXGIInfoQueue interface, IDXGIInfoQueue interface [DXGI],AddStorageFilterEntries method, IDXGIInfoQueue.AddStorageFilterEntries, IDXGIInfoQueue::AddStorageFilterEntries, direct3ddxgi.idxgiinfoqueue_addstoragefilterentries, dxgidebug/IDXGIInfoQueue::AddStorageFilterEntries
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
 - IDXGIInfoQueue.AddStorageFilterEntries
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIInfoQueue::AddStorageFilterEntries


## -description


Adds storage filters to the top of the storage-filter stack.


## -parameters




### -param Producer [in]

 A <a href="https://msdn.microsoft.com/85946D30-5E49-4E4B-AC25-394ABFF0DB11">DXGI_DEBUG_ID</a> value that identifies the entity that produced the filters.


### -param pFilter [in]

An array of <a href="https://msdn.microsoft.com/95E68ECE-39D2-4D16-9A8F-FE6E527A83E3">DXGI_INFO_QUEUE_FILTER</a> structures that describe the filters.


## -returns



Returns S_OK if successful; an error code otherwise. For a list of error codes, see <a href="https://msdn.microsoft.com/en-us/library/Bb509553(v=VS.85).aspx">DXGI_ERROR</a>.




## -remarks



<div class="alert"><b>Note</b>  This API requires the Windows Software Development Kit (SDK) for Windows 8.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/F1BC6752-F334-4E8C-BE42-B731635A799D">IDXGIInfoQueue</a>
 

 

