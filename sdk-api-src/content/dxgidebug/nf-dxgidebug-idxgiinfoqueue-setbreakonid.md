---
UID: NF:dxgidebug.IDXGIInfoQueue.SetBreakOnID
title: IDXGIInfoQueue::SetBreakOnID
author: windows-sdk-content
description: Sets a message identifier to break on when a message with that identifier passes through the storage filter.
old-location: direct3ddxgi\idxgiinfoqueue_setbreakonid.htm
tech.root: direct3ddxgi
ms.assetid: C225B262-B062-40D5-ADC0-491F47B111C9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDXGIInfoQueue interface [DXGI],SetBreakOnID method, IDXGIInfoQueue.SetBreakOnID, IDXGIInfoQueue::SetBreakOnID, SetBreakOnID, SetBreakOnID method [DXGI], SetBreakOnID method [DXGI],IDXGIInfoQueue interface, direct3ddxgi.idxgiinfoqueue_setbreakonid, dxgidebug/IDXGIInfoQueue::SetBreakOnID
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IDXGIInfoQueue.SetBreakOnID
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIInfoQueue::SetBreakOnID


## -description


Sets a message identifier to break on when a message with that identifier passes through the storage filter.


## -parameters




### -param Producer [in]

 A <a href="https://msdn.microsoft.com/85946D30-5E49-4E4B-AC25-394ABFF0DB11">DXGI_DEBUG_ID</a> value that identifies the entity that sets the breaking condition.


### -param ID [in]

An integer value that specifies the identifier of the message.


### -param bEnable [in]

A Boolean value that specifies whether <b>SetBreakOnID</b> turns on or off this breaking condition (<b>TRUE</b> for on, <b>FALSE</b> for off).


## -returns



Returns S_OK if successful; an error code otherwise. For a list of error codes, see <a href="https://msdn.microsoft.com/en-us/library/Bb509553(v=VS.85).aspx">DXGI_ERROR</a>.




## -remarks



<div class="alert"><b>Note</b>  This API requires the Windows Software Development Kit (SDK) for Windows 8.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/F1BC6752-F334-4E8C-BE42-B731635A799D">IDXGIInfoQueue</a>
 

 

