---
UID: NF:d3d12sdklayers.ID3D12DebugDevice1.SetDebugParameter
title: ID3D12DebugDevice1::SetDebugParameter (d3d12sdklayers.h)
author: windows-sdk-content
description: Modifies the D3D12 optional device-wide Debug Layer settings.
old-location: direct3d12\id3d12debugdevice1_setdebugparameter.htm
tech.root: direct3d12
ms.assetid: D97086C6-CED8-4C4E-ADA1-7A172B3202F3
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ID3D12DebugDevice1 interface,SetDebugParameter method, ID3D12DebugDevice1.SetDebugParameter, ID3D12DebugDevice1::SetDebugParameter, SetDebugParameter, SetDebugParameter method, SetDebugParameter method,ID3D12DebugDevice1 interface, d3d12sdklayers/ID3D12DebugDevice1::SetDebugParameter, direct3d12.id3d12debugdevice1_setdebugparameter
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
 - ID3D12DebugDevice1.SetDebugParameter
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D12DebugDevice1::SetDebugParameter


## -description


Modifies the D3D12 optional device-wide Debug Layer settings.


## -parameters




### -param Type

Type: <b><a href="https://msdn.microsoft.com/477155FF-9DF7-4E21-AF52-21EB3DBC3550">D3D12_DEBUG_DEVICE_PARAMETER_TYPE</a></b>

Specifies a <a href="https://msdn.microsoft.com/477155FF-9DF7-4E21-AF52-21EB3DBC3550">D3D12_DEBUG_DEVICE_PARAMETER_TYPE</a> value that indicates which debug parameter data to get.


### -param pData [in]

Type: <b>const void*</b>

Debug parameter data to set.


### -param DataSize

Type: <b>UINT</b>

Size in bytes of the data pointed to by <i>pData</i>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the <a href="https://msdn.microsoft.com/5F6CC962-7DB7-489F-82A4-9388313014D3">Direct3D 12 Return Codes</a>. 
          




## -see-also




<a href="https://msdn.microsoft.com/13A7E7D6-FF00-4E17-A7C5-C383F93F6A06">GetDebugParameter</a>



<a href="https://msdn.microsoft.com/DDB71272-195A-4E05-BA52-9EF858ACD6CB">ID3D12DebugDevice1</a>
 

 

