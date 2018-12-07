---
UID: NF:d3d10.ID3D10Device.VSSetShaderResources
title: ID3D10Device::VSSetShaderResources
author: windows-sdk-content
description: Bind an array of shader resources to the vertex shader stage.
old-location: direct3d10\id3d10device_vssetshaderresources.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10device_vssetshaderresources.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 28e716fb-c3fd-21d0-6820-b83de5a64caa, ID3D10Device interface [Direct3D 10],VSSetShaderResources method, ID3D10Device.VSSetShaderResources, ID3D10Device::VSSetShaderResources, VSSetShaderResources, VSSetShaderResources method [Direct3D 10], VSSetShaderResources method [Direct3D 10],ID3D10Device interface, d3d10/ID3D10Device::VSSetShaderResources, direct3d10.id3d10device_vssetshaderresources
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
 - ID3D10Device.VSSetShaderResources
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10Device::VSSetShaderResources


## -description


Bind an array of shader resources to the <a href="https://msdn.microsoft.com/en-us/library/Mt787172(v=VS.85).aspx">vertex shader stage</a>.


## -parameters




### -param StartSlot [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index into the device's zero-based array to begin setting shader resources to.


### -param NumViews [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Number of shader resources to set. Up to a maximum of 128 slots are available for shader resources.


### -param ppShaderResourceViews [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173854(v=VS.85).aspx">ID3D10ShaderResourceView</a>*</b>

Array of <a href="https://msdn.microsoft.com/en-us/library/Bb173854(v=VS.85).aspx">shader resource view</a> interfaces to set to the device.


## -returns



Returns nothing.




## -remarks



If you bind a subresource as an input and an output, this API will fill the destination shader resource slot with <b>NULL</b>. The debug layer (when active) will alert you if this is true.

For information about creating shader-resource views, see <a href="https://msdn.microsoft.com/en-us/library/Bb173558(v=VS.85).aspx">ID3D10Device::CreateShaderResourceView</a>.

The method will not hold a reference to the interfaces passed in. For that reason, applications should be careful not to release an interface currently in use by the device.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173528(v=VS.85).aspx">ID3D10Device Interface</a>
 

 

