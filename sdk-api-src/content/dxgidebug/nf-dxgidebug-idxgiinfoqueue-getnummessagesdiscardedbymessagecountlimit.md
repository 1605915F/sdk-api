---
UID: NF:dxgidebug.IDXGIInfoQueue.GetNumMessagesDiscardedByMessageCountLimit
title: IDXGIInfoQueue::GetNumMessagesDiscardedByMessageCountLimit (dxgidebug.h)
author: windows-sdk-content
description: Gets the number of messages that were discarded due to the message count limit.
old-location: direct3ddxgi\idxgiinfoqueue_getnummessagesdiscardedbymessagecountlimit.htm
tech.root: direct3ddxgi
ms.assetid: 8F97E69B-5534-409F-9702-9FC6D7940D65
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetNumMessagesDiscardedByMessageCountLimit, GetNumMessagesDiscardedByMessageCountLimit method [DXGI], GetNumMessagesDiscardedByMessageCountLimit method [DXGI],IDXGIInfoQueue interface, IDXGIInfoQueue interface [DXGI],GetNumMessagesDiscardedByMessageCountLimit method, IDXGIInfoQueue.GetNumMessagesDiscardedByMessageCountLimit, IDXGIInfoQueue::GetNumMessagesDiscardedByMessageCountLimit, direct3ddxgi.idxgiinfoqueue_getnummessagesdiscardedbymessagecountlimit, dxgidebug/IDXGIInfoQueue::GetNumMessagesDiscardedByMessageCountLimit
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
 - IDXGIInfoQueue.GetNumMessagesDiscardedByMessageCountLimit
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDXGIInfoQueue::GetNumMessagesDiscardedByMessageCountLimit


## -description


Gets the number of messages that were discarded due to the message count limit.


## -parameters




### -param Producer [in]

 A <a href="https://msdn.microsoft.com/85946D30-5E49-4E4B-AC25-394ABFF0DB11">DXGI_DEBUG_ID</a> value that identifies the entity that gets the number.


## -returns



Returns the number of messages that were discarded.




## -remarks



Get and set the message count limit with <a href="https://msdn.microsoft.com/F9700374-255D-423E-8E60-4FE7FFA9E807">IDXGIInfoQueue::GetMessageCountLimit</a> and <a href="https://msdn.microsoft.com/77FFF3EA-DEBC-4D92-9C10-E382CD663D20">IDXGIInfoQueue::SetMessageCountLimit</a>, respectively.



<div class="alert"><b>Note</b>  This API requires the Windows Software Development Kit (SDK) for Windows 8.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/F1BC6752-F334-4E8C-BE42-B731635A799D">IDXGIInfoQueue</a>
 

 

