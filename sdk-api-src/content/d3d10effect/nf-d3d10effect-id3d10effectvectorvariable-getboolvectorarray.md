---
UID: NF:d3d10effect.ID3D10EffectVectorVariable.GetBoolVectorArray
title: ID3D10EffectVectorVariable::GetBoolVectorArray
author: windows-sdk-content
description: Get an array of four-component vectors that contain boolean data.
old-location: direct3d10\id3d10effectvectorvariable_getboolvectorarray.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectvectorvariable_getboolvectorarray.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetBoolVectorArray, GetBoolVectorArray method [Direct3D 10], GetBoolVectorArray method [Direct3D 10],ID3D10EffectVectorVariable interface, ID3D10EffectVectorVariable interface [Direct3D 10],GetBoolVectorArray method, ID3D10EffectVectorVariable.GetBoolVectorArray, ID3D10EffectVectorVariable::GetBoolVectorArray, a6cfd4e9-ded5-2e31-f74b-352c828f9eb6, d3d10effect/ID3D10EffectVectorVariable::GetBoolVectorArray, direct3d10.id3d10effectvectorvariable_getboolvectorarray
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
 - ID3D10EffectVectorVariable.GetBoolVectorArray
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10EffectVectorVariable::GetBoolVectorArray


## -description


Get an array of four-component vectors that contain boolean data.


## -parameters




### -param pData [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a>*</b>

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




<a href="https://msdn.microsoft.com/en-us/library/Bb173748(v=VS.85).aspx">ID3D10EffectVectorVariable Interface</a>
 

 

