---
UID: NF:d3d10effect.ID3D10EffectVariable.AsBlend
title: ID3D10EffectVariable::AsBlend
author: windows-sdk-content
description: Get a effect-blend variable.
old-location: direct3d10\id3d10effectvariable_asblend.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectvariable_asblend.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AsBlend, AsBlend method [Direct3D 10], AsBlend method [Direct3D 10],ID3D10EffectVariable interface, ID3D10EffectVariable interface [Direct3D 10],AsBlend method, ID3D10EffectVariable.AsBlend, ID3D10EffectVariable::AsBlend, bc3da4a0-2ef6-7ffd-8a6d-1bf74e1ef7da, d3d10effect/ID3D10EffectVariable::AsBlend, direct3d10.id3d10effectvariable_asblend
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
 - ID3D10EffectVariable.AsBlend
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10EffectVariable::AsBlend


## -description


Get a effect-blend variable.


## -parameters






## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173631(v=VS.85).aspx">ID3D10EffectBlendVariable</a>*</b>

A pointer to an effect blend variable. See <a href="https://msdn.microsoft.com/en-us/library/Bb173631(v=VS.85).aspx">ID3D10EffectBlendVariable</a>.




## -remarks



AsBlend returns a version of the effect variable that has been specialized to an effect-blend variable. Similar to a cast, this specialization will return an invalid object if the effect variable does not contain effect-blend data.

Applications can test the returned object for validity by calling <a href="https://msdn.microsoft.com/en-us/library/Bb173746(v=VS.85).aspx">IsValid</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173724(v=VS.85).aspx">ID3D10EffectVariable Interface</a>
 

 

