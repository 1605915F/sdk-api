---
UID: NF:d3d12sdklayers.ID3D12InfoQueue.SetBreakOnCategory
title: ID3D12InfoQueue::SetBreakOnCategory
author: windows-sdk-content
description: Set a message category to break on when a message with that category passes through the storage filter.
old-location: direct3d12\id3d12infoqueue_setbreakoncategory.htm
tech.root: direct3d12
ms.assetid: BE56C85A-3FCE-4EC6-B42C-DF0187237AC5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3D12InfoQueue interface,SetBreakOnCategory method, ID3D12InfoQueue.SetBreakOnCategory, ID3D12InfoQueue::SetBreakOnCategory, SetBreakOnCategory, SetBreakOnCategory method, SetBreakOnCategory method,ID3D12InfoQueue interface, d3d12sdklayers/ID3D12InfoQueue::SetBreakOnCategory, direct3d12.id3d12infoqueue_setbreakoncategory
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ID3D12InfoQueue.SetBreakOnCategory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12InfoQueue::SetBreakOnCategory


## -description


Set a message category to break on when a message with that category passes through the storage filter.




## -parameters




### -param Category [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn950145(v=VS.85).aspx">D3D12_MESSAGE_CATEGORY</a></b>

Message category to break on.
          


### -param bEnable [in]

Type: <b>BOOL</b>

Turns this breaking condition on or off (true for on, false for off).


          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the <a href="https://msdn.microsoft.com/en-us/library/Dn706075(v=VS.85).aspx">Direct3D 12 Return Codes</a>. 
          




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn950163(v=VS.85).aspx">ID3D12InfoQueue</a>
 

 

