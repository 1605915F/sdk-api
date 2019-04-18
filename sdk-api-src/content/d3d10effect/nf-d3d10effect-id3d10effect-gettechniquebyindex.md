---
UID: NF:d3d10effect.ID3D10Effect.GetTechniqueByIndex
title: ID3D10Effect::GetTechniqueByIndex (d3d10effect.h)
author: windows-sdk-content
description: Get a technique by index.
old-location: direct3d10\id3d10effect_gettechniquebyindex.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effect_gettechniquebyindex.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: GetTechniqueByIndex, GetTechniqueByIndex method [Direct3D 10], GetTechniqueByIndex method [Direct3D 10],ID3D10Effect interface, ID3D10Effect interface [Direct3D 10],GetTechniqueByIndex method, ID3D10Effect.GetTechniqueByIndex, ID3D10Effect::GetTechniqueByIndex, d3d10effect/ID3D10Effect::GetTechniqueByIndex, direct3d10.id3d10effect_gettechniquebyindex, fa1352dd-acaf-8d2f-cb41-b99cf103e21b
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
 - ID3D10Effect.GetTechniqueByIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10Effect::GetTechniqueByIndex


## -description


Get a technique by index.


## -parameters




### -param Index [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

A zero-based index.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173708(v=VS.85).aspx">ID3D10EffectTechnique</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/en-us/library/Bb173708(v=VS.85).aspx">ID3D10EffectTechnique Interface</a>.




## -remarks



An effect contains one or more techniques; each technique contains one or more passes. You can access a technique using its name or with an index. 
      For more about techniques, see <a href="https://msdn.microsoft.com/en-us/library/Bb205112(v=VS.85).aspx">techniques and passes</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173630(v=VS.85).aspx">ID3D10Effect Interface</a>
 

 

