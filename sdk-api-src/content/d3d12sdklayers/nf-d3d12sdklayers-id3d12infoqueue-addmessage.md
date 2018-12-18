---
UID: NF:d3d12sdklayers.ID3D12InfoQueue.AddMessage
title: ID3D12InfoQueue::AddMessage
author: windows-sdk-content
description: Adds a debug message to the message queue and sends that message to debug output.
old-location: direct3d12\id3d12infoqueue_addmessage.htm
tech.root: direct3d12
ms.assetid: 34AAF9BB-5340-4DB3-87B9-6C26AB6C881C
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddMessage, AddMessage method, AddMessage method,ID3D12InfoQueue interface, ID3D12InfoQueue interface,AddMessage method, ID3D12InfoQueue.AddMessage, ID3D12InfoQueue::AddMessage, d3d12sdklayers/ID3D12InfoQueue::AddMessage, direct3d12.id3d12infoqueue_addmessage
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
 - ID3D12InfoQueue.AddMessage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12InfoQueue::AddMessage


## -description


Adds a debug message to the message queue and sends that message to debug output.




## -parameters




### -param Category [in]

Type: <b><a href="https://msdn.microsoft.com/297923A3-CE6A-46AF-B8B6-E2AE0C1920CC">D3D12_MESSAGE_CATEGORY</a></b>

Category of a message.


          


### -param Severity [in]

Type: <b><a href="https://msdn.microsoft.com/44D94C37-4BA8-49FC-BEEF-6666AD59B627">D3D12_MESSAGE_SEVERITY</a></b>

Severity of a message.


          


### -param ID [in]

Type: <b><a href="https://msdn.microsoft.com/95681EB0-C00B-42C8-91E1-1D1F657C886B">D3D12_MESSAGE_ID</a></b>

Unique identifier of a message.




### -param pDescription [in]

Type: <b>LPCSTR</b>

User-defined message.




## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the <a href="https://msdn.microsoft.com/5F6CC962-7DB7-489F-82A4-9388313014D3">Direct3D 12 Return Codes</a>. 
          




## -remarks



This method is used by the runtime's internal mechanisms to add debug messages to the message queue and send them to debug output. For applications to add their own custom messages to the message queue and send them to debug output, call <a href="https://msdn.microsoft.com/C5979BF4-C44D-461F-8FAB-D0577691C5BF">ID3D12InfoQueue::AddApplicationMessage</a>.






## -see-also




<a href="https://msdn.microsoft.com/61667AAC-05AC-4745-8992-E9377641D411">ID3D12InfoQueue</a>
 

 

