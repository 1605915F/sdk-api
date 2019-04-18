---
UID: NF:d3d12sdklayers.ID3D12InfoQueue.GetBreakOnCategory
title: ID3D12InfoQueue::GetBreakOnCategory (d3d12sdklayers.h)
author: windows-sdk-content
description: Get a message category to break on when a message with that category passes through the storage filter.
old-location: direct3d12\id3d12infoqueue_getbreakoncategory.htm
tech.root: direct3d12
ms.assetid: 3B966BB5-4AA6-4475-890F-4477A5C7E55E
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetBreakOnCategory, GetBreakOnCategory method, GetBreakOnCategory method,ID3D12InfoQueue interface, ID3D12InfoQueue interface,GetBreakOnCategory method, ID3D12InfoQueue.GetBreakOnCategory, ID3D12InfoQueue::GetBreakOnCategory, d3d12sdklayers/ID3D12InfoQueue::GetBreakOnCategory, direct3d12.id3d12infoqueue_getbreakoncategory
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
 - ID3D12InfoQueue.GetBreakOnCategory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D12InfoQueue::GetBreakOnCategory


## -description


Get a message category to break on when a message with that category passes through the storage filter.




## -parameters




### -param Category [in]

Type: <b><a href="https://msdn.microsoft.com/297923A3-CE6A-46AF-B8B6-E2AE0C1920CC">D3D12_MESSAGE_CATEGORY</a></b>

Message category to break on.
          


## -returns



Type: <b>BOOL</b>

Whether this breaking condition is turned on or off (true for on, false for off).






## -see-also




<a href="https://msdn.microsoft.com/61667AAC-05AC-4745-8992-E9377641D411">ID3D12InfoQueue</a>
 

 

