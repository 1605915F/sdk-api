---
UID: NF:d3d10.ID3D10Device.SetPrivateData
title: ID3D10Device::SetPrivateData
author: windows-sdk-content
description: Set data to a device and associate that data with a guid.
old-location: direct3d10\id3d10device_setprivatedata.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10device_setprivatedata.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID3D10Device interface [Direct3D 10],SetPrivateData method, ID3D10Device.SetPrivateData, ID3D10Device::SetPrivateData, SetPrivateData, SetPrivateData method [Direct3D 10], SetPrivateData method [Direct3D 10],ID3D10Device interface, d3d10/ID3D10Device::SetPrivateData, direct3d10.id3d10device_setprivatedata, eaeabbc7-7fa6-0ea4-315b-75d083b44da6
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d10.h
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
req.lib: D3D10.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D10.lib
 - D3D10.dll
api_name:
 - ID3D10Device.SetPrivateData
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10Device::SetPrivateData


## -description


Set data to a device and associate that data with a guid.


## -parameters




### -param guid [in]

Type: <b><a href="http://msdn.microsoft.com/en-us/library/cc237815(PROT.13).aspx">REFGUID</a></b>

Guid associated with the data.


### -param DataSize [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

Size of the data.


### -param pData [in]

Type: <b>const void*</b>

Pointer to the data to be stored with this device. If pData is <b>NULL</b>, DataSize must also be 0, and any data previously associated with the guid will be destroyed.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method returns one of the following <a href="https://msdn.microsoft.com/en-us/library/Bb205278(v=VS.85).aspx">Direct3D 10 Return Codes</a>.




## -remarks



The data stored in the device with this method can be retrieved with <a href="https://msdn.microsoft.com/en-us/library/Bb173574(v=VS.85).aspx">ID3D10DeviceChild::GetPrivateData</a>.

The data and guid set with this method will typically be application-defined.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173528(v=VS.85).aspx">ID3D10Device Interface</a>
 

 

