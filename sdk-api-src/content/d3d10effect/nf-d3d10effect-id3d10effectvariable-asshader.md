---
UID: NF:d3d10effect.ID3D10EffectVariable.AsShader
title: ID3D10EffectVariable::AsShader
author: windows-sdk-content
description: Get a shader variable.
old-location: direct3d10\id3d10effectvariable_asshader.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectvariable_asshader.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AsShader, AsShader method [Direct3D 10], AsShader method [Direct3D 10],ID3D10EffectVariable interface, ID3D10EffectVariable interface [Direct3D 10],AsShader method, ID3D10EffectVariable.AsShader, ID3D10EffectVariable::AsShader, cfb94875-697a-f808-87e1-768dc74cc207, d3d10effect/ID3D10EffectVariable::AsShader, direct3d10.id3d10effectvariable_asshader
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - ID3D10EffectVariable.AsShader
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10EffectVariable::AsShader


## -description


Get a shader variable.


## -parameters






## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173698(v=VS.85).aspx">ID3D10EffectShaderVariable</a>*</b>

A pointer to a shader variable. See <a href="https://msdn.microsoft.com/en-us/library/Bb173698(v=VS.85).aspx">ID3D10EffectShaderVariable</a>.




## -remarks



AsShader returns a version of the effect variable that has been specialized to a shader variable. Similar to a cast, this specialization will return an invalid object if the effect variable does not contain shader data.

Applications can test the returned object for validity by calling <a href="https://msdn.microsoft.com/en-us/library/Bb173746(v=VS.85).aspx">IsValid</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173724(v=VS.85).aspx">ID3D10EffectVariable Interface</a>
 

 

