---
UID: NF:d3d11.ID3D11SamplerState.GetDesc
title: ID3D11SamplerState::GetDesc
author: windows-sdk-content
description: Gets the description for sampler state that you used to create the sampler-state object.
old-location: direct3d11\id3d11samplerstate_getdesc.htm
tech.root: direct3d11
ms.assetid: cca7f0f1-44b7-4f49-9149-acb12d745890
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 3558faeb-2890-903a-fe84-4afdeb705f2b, GetDesc, GetDesc method [Direct3D 11], GetDesc method [Direct3D 11],ID3D11SamplerState interface, ID3D11SamplerState interface [Direct3D 11],GetDesc method, ID3D11SamplerState.GetDesc, ID3D11SamplerState::GetDesc, d3d11/ID3D11SamplerState::GetDesc, direct3d11.id3d11samplerstate_getdesc
ms.topic: method
req.header: d3d11.h
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
req.lib: D3D11.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D11.lib
 - D3D11.dll
api_name:
 - ID3D11SamplerState.GetDesc
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11SamplerState::GetDesc


## -description


Gets the description for sampler state that you used to create the sampler-state object.


## -parameters




### -param pDesc [out]

Type: <b><a href="https://msdn.microsoft.com/97dd6cac-6657-4a1e-b631-4e5d36994b16">D3D11_SAMPLER_DESC</a>*</b>

A pointer to a <a href="https://msdn.microsoft.com/97dd6cac-6657-4a1e-b631-4e5d36994b16">D3D11_SAMPLER_DESC</a> structure that receives a description of the sampler state.


## -returns



Returns nothing.




## -remarks



You use the description for sampler state in a call to the <a href="https://msdn.microsoft.com/66cf7189-2882-43a4-8732-657402c983db">ID3D11Device::CreateSamplerState</a> method to create the sampler-state object.




## -see-also




<a href="https://msdn.microsoft.com/8dc2facc-4f51-4064-aab4-028a06b9d7e6">ID3D11SamplerState</a>
 

 

