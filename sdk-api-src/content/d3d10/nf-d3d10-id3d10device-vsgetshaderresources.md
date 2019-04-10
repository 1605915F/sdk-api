---
UID: NF:d3d10.ID3D10Device.VSGetShaderResources
title: ID3D10Device::VSGetShaderResources (d3d10.h)
author: windows-sdk-content
description: Get the vertex shader resources.
old-location: direct3d10\id3d10device_vsgetshaderresources.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10device_vsgetshaderresources.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 55f36c24-a1d1-912f-485e-13d633bf3178, ID3D10Device interface [Direct3D 10],VSGetShaderResources method, ID3D10Device.VSGetShaderResources, ID3D10Device::VSGetShaderResources, VSGetShaderResources, VSGetShaderResources method [Direct3D 10], VSGetShaderResources method [Direct3D 10],ID3D10Device interface, d3d10/ID3D10Device::VSGetShaderResources, direct3d10.id3d10device_vsgetshaderresources
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
 - ID3D10Device.VSGetShaderResources
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10Device::VSGetShaderResources


## -description


Get the vertex shader resources.


## -parameters




### -param StartSlot [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index into the device's zero-based array to begin getting shader resources from.


### -param NumViews [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of resources to get from the device. Up to a maximum of 128 slots are available for shader resources.


### -param ppShaderResourceViews [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173854(v=VS.85).aspx">ID3D10ShaderResourceView</a>**</b>

Array of <a href="https://msdn.microsoft.com/en-us/library/Bb173854(v=VS.85).aspx">shader resource view</a> interfaces to be returned by the device.


## -returns



Returns nothing.




## -remarks



Any returned interfaces will have their reference count incremented by one. Applications should call <a href="http://msdn.microsoft.com/en-us/library/ms682317(VS.85).aspx">IUnknown::Release</a> on the returned interfaces when they are no longer needed to avoid memory leaks.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173528(v=VS.85).aspx">ID3D10Device Interface</a>
 

 

