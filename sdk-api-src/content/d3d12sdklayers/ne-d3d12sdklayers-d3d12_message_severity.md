---
UID: NE:d3d12sdklayers.D3D12_MESSAGE_SEVERITY
title: D3D12_MESSAGE_SEVERITY (d3d12sdklayers.h)
author: windows-sdk-content
description: Debug message severity levels for an information queue.
old-location: direct3d12\d3d12_message_severity.htm
tech.root: direct3d12
ms.assetid: 44D94C37-4BA8-49FC-BEEF-6666AD59B627
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: D3D12_MESSAGE_SEVERITY, D3D12_MESSAGE_SEVERITY enumeration, D3D12_MESSAGE_SEVERITY_CORRUPTION, D3D12_MESSAGE_SEVERITY_ERROR, D3D12_MESSAGE_SEVERITY_INFO, D3D12_MESSAGE_SEVERITY_MESSAGE, D3D12_MESSAGE_SEVERITY_WARNING, d3d12sdklayers/D3D12_MESSAGE_SEVERITY, d3d12sdklayers/D3D12_MESSAGE_SEVERITY_CORRUPTION, d3d12sdklayers/D3D12_MESSAGE_SEVERITY_ERROR, d3d12sdklayers/D3D12_MESSAGE_SEVERITY_INFO, d3d12sdklayers/D3D12_MESSAGE_SEVERITY_MESSAGE, d3d12sdklayers/D3D12_MESSAGE_SEVERITY_WARNING, direct3d12.d3d12_message_severity
ms.topic: enum
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
 - HeaderDef
api_location:
 - d3d12sdklayers.h
api_name:
 - D3D12_MESSAGE_SEVERITY
product: Windows
targetos: Windows
req.typenames: D3D12_MESSAGE_SEVERITY
req.redist: 
ms.custom: 19H1
---

# D3D12_MESSAGE_SEVERITY enumeration


## -description


Debug message severity levels for an information queue.


## -enum-fields




### -field D3D12_MESSAGE_SEVERITY_CORRUPTION

Indicates a corruption error.
          


### -field D3D12_MESSAGE_SEVERITY_ERROR

Indicates an error.
          


### -field D3D12_MESSAGE_SEVERITY_WARNING

Indicates a warning.
          


### -field D3D12_MESSAGE_SEVERITY_INFO

Indicates an information message.
          


### -field D3D12_MESSAGE_SEVERITY_MESSAGE

Indicates a message other than corruption, error, warning or information.
          


## -remarks



Use these values to allow or deny message categories to pass through the storage and retrieval filters for an information queue (see <a href="https://msdn.microsoft.com/5CD64E71-8530-43FB-B441-25C61ED6F317">D3D12_INFO_QUEUE_FILTER</a>). This API is used by <a href="https://msdn.microsoft.com/C5979BF4-C44D-461F-8FAB-D0577691C5BF">AddApplicationMessage</a> and <a href="https://msdn.microsoft.com/34AAF9BB-5340-4DB3-87B9-6C26AB6C881C">AddMessage</a>.


        




## -see-also




<a href="https://msdn.microsoft.com/6E76C857-128E-4F0E-9711-72C4CF6C835C">Debug Layer Enumerations</a>
 

 

