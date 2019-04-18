---
UID: NF:d3d10effect.ID3D10EffectScalarVariable.SetIntArray
title: ID3D10EffectScalarVariable::SetIntArray (d3d10effect.h)
author: windows-sdk-content
description: Set an array of integer variables.
old-location: direct3d10\id3d10effectscalarvariable_setintarray.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectscalarvariable_setintarray.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 557a34dc-1dce-4cb2-5269-cebf5fc86f76, ID3D10EffectScalarVariable interface [Direct3D 10],SetIntArray method, ID3D10EffectScalarVariable.SetIntArray, ID3D10EffectScalarVariable::SetIntArray, SetIntArray, SetIntArray method [Direct3D 10], SetIntArray method [Direct3D 10],ID3D10EffectScalarVariable interface, d3d10effect/ID3D10EffectScalarVariable::SetIntArray, direct3d10.id3d10effectscalarvariable_setintarray
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
 - ID3D10EffectScalarVariable.SetIntArray
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10EffectScalarVariable::SetIntArray


## -description


Set an array of integer variables.


## -parameters




### -param pData [in]

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
 

 

