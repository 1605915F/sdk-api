---
UID: NF:d3d10effect.ID3D10EffectScalarVariable.GetIntArray
title: ID3D10EffectScalarVariable::GetIntArray (d3d10effect.h)
author: windows-sdk-content
description: Get an array of integer variables.
old-location: direct3d10\id3d10effectscalarvariable_getintarray.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectscalarvariable_getintarray.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 3b56ed87-da9a-3aec-33c5-66ed69d44a04, GetIntArray, GetIntArray method [Direct3D 10], GetIntArray method [Direct3D 10],ID3D10EffectScalarVariable interface, ID3D10EffectScalarVariable interface [Direct3D 10],GetIntArray method, ID3D10EffectScalarVariable.GetIntArray, ID3D10EffectScalarVariable::GetIntArray, d3d10effect/ID3D10EffectScalarVariable::GetIntArray, direct3d10.id3d10effectscalarvariable_getintarray
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
 - ID3D10EffectScalarVariable.GetIntArray
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10EffectScalarVariable::GetIntArray


## -description


Get an array of integer variables.


## -parameters




### -param pData [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">int</a>*</b>

A pointer to the start of the data to set.


### -param Offset [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Must be set to 0; this is reserved for future use. 


### -param Count [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of array elements to set.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Returns one of the following <a href="https://msdn.microsoft.com/en-us/library/Bb205278(v=VS.85).aspx">Direct3D 10 Return Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173680(v=VS.85).aspx">ID3D10EffectScalarVariable Interface</a>
 

 

