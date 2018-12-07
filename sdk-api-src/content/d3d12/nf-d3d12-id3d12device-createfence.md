---
UID: NF:d3d12.ID3D12Device.CreateFence
title: ID3D12Device::CreateFence
author: windows-sdk-content
description: Creates a fence object.
old-location: direct3d12\id3d12device_createfence.htm
tech.root: direct3d12
ms.assetid: 731A60CA-644A-4FC2-8461-DDD686363BED
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateFence, CreateFence method, CreateFence method,ID3D12Device interface, ID3D12Device interface,CreateFence method, ID3D12Device.CreateFence, ID3D12Device::CreateFence, d3d12/ID3D12Device::CreateFence, direct3d12.id3d12device_createfence
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d12.h
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
req.lib: D3D12.lib
req.dll: D3D12.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D12.dll
api_name:
 - ID3D12Device.CreateFence
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12Device::CreateFence


## -description


Creates a fence object.
        


## -parameters




### -param InitialValue

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT64</a></b>

The initial value for the fence.
          


### -param Flags

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn986729(v=VS.85).aspx">D3D12_FENCE_FLAGS</a></b>

A combination of <a href="https://msdn.microsoft.com/en-us/library/Dn986729(v=VS.85).aspx">D3D12_FENCE_FLAGS</a>-typed values that are combined by using a bitwise OR operation. 
            The resulting value specifies options for the fence.
          


### -param riid

Type: <b>REFIID</b>

The globally unique identifier (<b>GUID</b>) for the fence interface (<a href="https://msdn.microsoft.com/en-us/library/Dn899188(v=VS.85).aspx">ID3D12Fence</a>).
            The <b>REFIID</b>, or <b>GUID</b>, of the interface to the fence can be obtained by using the __uuidof() macro.
            For example, __uuidof(ID3D12Fence) will get the <b>GUID</b> of the interface to a fence.
          


### -param ppFence [out]

Type: <b>void**</b>

A pointer to a memory block that receives a pointer to the <a href="https://msdn.microsoft.com/en-us/library/Dn899188(v=VS.85).aspx">ID3D12Fence</a> interface that is used to access the fence.
          


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">HRESULT</a></b>

Returns <b>S_OK</b> if successful; otherwise, returns one of the <a href="https://msdn.microsoft.com/en-us/library/Dn706075(v=VS.85).aspx">Direct3D 12 Return Codes</a>.
          




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn788650(v=VS.85).aspx">ID3D12Device</a>
 

 

