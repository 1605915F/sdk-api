---
UID: NF:d3d11shader.ID3D11ModuleInstance.BindSampler
title: ID3D11ModuleInstance::BindSampler
author: windows-sdk-content
description: Rebinds a sampler from source slot to destination slot.
old-location: direct3d11\id3d11moduleinstance_bindsampler.htm
tech.root: direct3d11
ms.assetid: FB7A63DE-C8EC-456D-84D6-D0AF682A46E8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BindSampler, BindSampler method [Direct3D 11], BindSampler method [Direct3D 11],ID3D11ModuleInstance interface, ID3D11ModuleInstance interface [Direct3D 11],BindSampler method, ID3D11ModuleInstance.BindSampler, ID3D11ModuleInstance::BindSampler, d3d11shader/ID3D11ModuleInstance::BindSampler, direct3d11.id3d11moduleinstance_bindsampler
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d11shader.h
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
req.lib: D3DCompiler.lib
req.dll: D3DCompiler_47.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3DCompiler_47.dll
api_name:
 - ID3D11ModuleInstance.BindSampler
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11ModuleInstance::BindSampler


## -description


Rebinds a sampler from source slot to destination slot.


## -parameters




### -param uSrcSlot [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

The first source slot number for rebinding.


### -param uDstSlot [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

The first destination slot number for rebinding.


### -param uCount [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx">UINT</a></b>

The number of slots for rebinding. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns:

<ul>
<li><b>S_OK</b> for a valid rebinding</li>
<li><b>S_FALSE</b> for rebinding a nonexistent slot; that is, for which the shader reflection doesn’t have any data</li>
<li><b>E_FAIL</b> for an invalid rebinding, for example, the rebinding is out-of-bounds</li>
<li>Possibly one of the other <a href="https://msdn.microsoft.com/en-us/library/Ff476174(v=VS.85).aspx">Direct3D 11 Return Codes</a>
</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn280564(v=VS.85).aspx">ID3D11ModuleInstance</a>
 

 

