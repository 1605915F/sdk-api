---
UID: NF:d3d10sdklayers.ID3D10InfoQueue.GetMessage
title: ID3D10InfoQueue::GetMessage (d3d10sdklayers.h)
author: windows-sdk-content
description: Get a message from the message queue.
old-location: direct3d10\id3d10infoqueue_getmessage.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10infoqueue_getmessage.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 792ee245-051d-ca89-58b7-8d2ebfaf48b6, GetMessage, GetMessage method [Direct3D 10], GetMessage method [Direct3D 10],ID3D10InfoQueue interface, ID3D10InfoQueue interface [Direct3D 10],GetMessage method, ID3D10InfoQueue.GetMessage, ID3D10InfoQueue::GetMessage, d3d10sdklayers/ID3D10InfoQueue::GetMessage, direct3d10.id3d10infoqueue_getmessage
ms.topic: method
req.header: d3d10sdklayers.h
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
 - D3D10SDKLayers.h
api_name:
 - ID3D10InfoQueue.GetMessage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10InfoQueue::GetMessage


## -description


Get a message from the message queue.


## -parameters




### -param MessageIndex [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT64</a></b>

Index into message queue after an optional retrieval filter has been applied. This can be between 0 and the number of messages in the message queue that pass through the retrieval filter (which can be obtained with <a href="https://msdn.microsoft.com/en-us/library/Bb173797(v=VS.85).aspx">ID3D10InfoQueue::GetNumStoredMessagesAllowedByRetrievalFilter</a>). 0 is the message at the front of the message queue.


### -param pMessage [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205322(v=VS.85).aspx">D3D10_MESSAGE</a>*</b>

Returned message (see <a href="https://msdn.microsoft.com/en-us/library/Bb205322(v=VS.85).aspx">D3D10_MESSAGE</a>).


### -param pMessageByteLength [in, out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">SIZE_T</a>*</b>

Size of pMessage in bytes, including the size of the message string that the pMessage points to.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the following <a href="https://msdn.microsoft.com/en-us/library/Bb205278(v=VS.85).aspx">Direct3D 10 Return Codes</a>.




## -remarks



This method does not remove any messages from the message queue.

This method gets messages from the message queue after an optional retrieval filter has been applied.

Applications should call this method twice to retrieve a message - first to obtain the size of the message and second to get the message. Here is a typical example:


```

// Get the size of the message
SIZE_T messageLength = 0;
HRESULT hr = pInfoQueue->GetMessage(0, NULL, &messageLength);

// Allocate space and get the message
D3D10_MESSAGE * pMessage = (D3D10_MESSAGE*)malloc(messageLength);
hr = pInfoQueue->GetMessage(0, pMessage, &messageLength);

```


For an overview see <a href="https://msdn.microsoft.com/en-us/library/Bb173779(v=VS.85).aspx">Information Queue Overview</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173779(v=VS.85).aspx">ID3D10InfoQueue Interface</a>
 

 

