---
UID: NF:d3d12sdklayers.ID3D12InfoQueue.AddApplicationMessage
title: ID3D12InfoQueue::AddApplicationMessage
author: windows-sdk-content
description: Adds a user-defined message to the message queue and sends that message to debug output.
old-location: direct3d12\id3d12infoqueue_addapplicationmessage.htm
tech.root: direct3d12
ms.assetid: C5979BF4-C44D-461F-8FAB-D0577691C5BF
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddApplicationMessage, AddApplicationMessage method, AddApplicationMessage method,ID3D12InfoQueue interface, ID3D12InfoQueue interface,AddApplicationMessage method, ID3D12InfoQueue.AddApplicationMessage, ID3D12InfoQueue::AddApplicationMessage, d3d12sdklayers/ID3D12InfoQueue::AddApplicationMessage, direct3d12.id3d12infoqueue_addapplicationmessage
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
 - ID3D12InfoQueue.AddApplicationMessage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12InfoQueue::AddApplicationMessage


## -description


Adds a user-defined message to the message queue and sends that message to debug output.




## -parameters




### -param Severity [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn950147(v=VS.85).aspx">D3D12_MESSAGE_SEVERITY</a></b>

Severity of a message.


### -param pDescription [in]

Type: <b>LPCSTR</b>

Specifies the message string.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the <a href="https://msdn.microsoft.com/en-us/library/Dn706075(v=VS.85).aspx">Direct3D 12 Return Codes</a>. 
          




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn950163(v=VS.85).aspx">ID3D12InfoQueue</a>
 

 

