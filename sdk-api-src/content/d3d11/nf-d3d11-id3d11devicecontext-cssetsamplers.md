---
UID: NF:d3d11.ID3D11DeviceContext.CSSetSamplers
title: ID3D11DeviceContext::CSSetSamplers
author: windows-sdk-content
description: Set an array of sampler states to the compute-shader stage.
old-location: direct3d11\id3d11devicecontext_cssetsamplers.htm
tech.root: direct3d11
ms.assetid: 8b7f5c6d-0d9d-4b8b-a812-1e2b3b7386e9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CSSetSamplers, CSSetSamplers method [Direct3D 11], CSSetSamplers method [Direct3D 11],ID3D11DeviceContext interface, ID3D11DeviceContext interface [Direct3D 11],CSSetSamplers method, ID3D11DeviceContext.CSSetSamplers, ID3D11DeviceContext::CSSetSamplers, aa74392c-a8c7-cf2c-b761-f00d5b5b4fb9, d3d11/ID3D11DeviceContext::CSSetSamplers, direct3d11.id3d11devicecontext_cssetsamplers
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
 - ID3D11DeviceContext.CSSetSamplers
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D11DeviceContext::CSSetSamplers


## -description


Set an array of sampler states to the compute-shader stage.


## -parameters




### -param StartSlot [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index into the device's zero-based array to begin setting samplers to (ranges from 0 to D3D11_COMMONSHADER_SAMPLER_SLOT_COUNT - 1).


### -param NumSamplers [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Number of samplers in the array. Each pipeline stage has a total of 16 sampler slots available (ranges from 0 to D3D11_COMMONSHADER_SAMPLER_SLOT_COUNT - StartSlot).


### -param ppSamplers [in, optional]

Type: <b><a href="https://msdn.microsoft.com/8dc2facc-4f51-4064-aab4-028a06b9d7e6">ID3D11SamplerState</a>*</b>

Pointer to an array of sampler-state interfaces (see <a href="https://msdn.microsoft.com/8dc2facc-4f51-4064-aab4-028a06b9d7e6">ID3D11SamplerState</a>). See Remarks.


## -returns



This method does not return a value.




## -remarks



Any sampler may be set to <b>NULL</b>; this invokes the default state, which is defined to be the following.

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>//Default sampler state:
D3D11_SAMPLER_DESC SamplerDesc;
SamplerDesc.Filter = D3D11_FILTER_MIN_MAG_MIP_LINEAR;
SamplerDesc.AddressU = D3D11_TEXTURE_ADDRESS_CLAMP;
SamplerDesc.AddressV = D3D11_TEXTURE_ADDRESS_CLAMP;
SamplerDesc.AddressW = D3D11_TEXTURE_ADDRESS_CLAMP;
SamplerDesc.MipLODBias = 0;
SamplerDesc.MaxAnisotropy = 1;
SamplerDesc.ComparisonFunc = D3D11_COMPARISON_NEVER;
SamplerDesc.BorderColor[0] = 1.0f;
SamplerDesc.BorderColor[1] = 1.0f;
SamplerDesc.BorderColor[2] = 1.0f;
SamplerDesc.BorderColor[3] = 1.0f;
SamplerDesc.MinLOD = -FLT_MAX;
SamplerDesc.MaxLOD = FLT_MAX;
		</pre>
</td>
</tr>
</table></span></div>
The method will hold a reference to the interfaces passed in.
      This differs from the device state behavior in Direct3D 10.




## -see-also




<a href="https://msdn.microsoft.com/afb32c09-77f2-4c33-bd93-8dce92a2e45e">ID3D11DeviceContext</a>
 

 

