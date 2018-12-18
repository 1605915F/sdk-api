---
UID: NF:d3d12sdklayers.ID3D12InfoQueue.GetBreakOnID
title: ID3D12InfoQueue::GetBreakOnID
author: windows-sdk-content
description: Get a message identifier to break on when a message with that identifier passes through the storage filter.
old-location: direct3d12\id3d12infoqueue_getbreakonid.htm
tech.root: direct3d12
ms.assetid: 04763E09-3076-4865-8026-976ED08B61C3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetBreakOnID, GetBreakOnID method, GetBreakOnID method,ID3D12InfoQueue interface, ID3D12InfoQueue interface,GetBreakOnID method, ID3D12InfoQueue.GetBreakOnID, ID3D12InfoQueue::GetBreakOnID, d3d12sdklayers/ID3D12InfoQueue::GetBreakOnID, direct3d12.id3d12infoqueue_getbreakonid
ms.topic: method
req.header: d3d12sdklayers.h
req.include-header: 
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
 - COM
api_location:
 - d3d12sdklayers.h
api_name:
 - ID3D12InfoQueue.GetBreakOnID
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12InfoQueue::GetBreakOnID


## -description


Get a message identifier to break on when a message with that identifier passes through the storage filter.




## -parameters




### -param ID [in]

Type: <b><a href="https://msdn.microsoft.com/95681EB0-C00B-42C8-91E1-1D1F657C886B">D3D12_MESSAGE_ID</a></b>

Message identifier to break on.
          


## -returns



Type: <b>BOOL</b>

Whether this breaking condition is turned on or off (true for on, false for off).






## -see-also




<a href="https://msdn.microsoft.com/61667AAC-05AC-4745-8992-E9377641D411">ID3D12InfoQueue</a>
 

 

