---
UID: NF:d3d10effect.ID3D10EffectSamplerVariable.GetSampler
title: ID3D10EffectSamplerVariable::GetSampler (d3d10effect.h)
author: windows-sdk-content
description: Get a pointer to a sampler interface.
old-location: direct3d10\id3d10effectsamplervariable_getsampler.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectsamplervariable_getsampler.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetSampler, GetSampler method [Direct3D 10], GetSampler method [Direct3D 10],ID3D10EffectSamplerVariable interface, ID3D10EffectSamplerVariable interface [Direct3D 10],GetSampler method, ID3D10EffectSamplerVariable.GetSampler, ID3D10EffectSamplerVariable::GetSampler, cd07e1d0-28d4-ba10-87d9-3768dd4f0157, d3d10effect/ID3D10EffectSamplerVariable::GetSampler, direct3d10.id3d10effectsamplervariable_getsampler
ms.topic: method
req.header: d3d10effect.h
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
 - D3D10Effect.h
api_name:
 - ID3D10EffectSamplerVariable.GetSampler
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10EffectSamplerVariable::GetSampler


## -description


Get a pointer to a sampler interface.


## -parameters




### -param Index [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index into an array of sampler interfaces. If there is only one sampler interface, use 0.


### -param ppSampler [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173833(v=VS.85).aspx">ID3D10SamplerState</a>**</b>

The address of a pointer to a sampler interface (see <a href="https://msdn.microsoft.com/en-us/library/Bb173833(v=VS.85).aspx">ID3D10SamplerState Interface</a>).


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns one of the following <a href="https://msdn.microsoft.com/en-us/library/Bb205278(v=VS.85).aspx">Direct3D 10 Return Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173677(v=VS.85).aspx">ID3D10EffectSamplerVariable Interface</a>
 

 

