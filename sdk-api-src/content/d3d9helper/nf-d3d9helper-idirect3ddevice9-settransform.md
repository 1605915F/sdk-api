---
UID: NF:d3d9helper.IDirect3DDevice9.SetTransform
title: IDirect3DDevice9::SetTransform (d3d9helper.h)
author: windows-sdk-content
description: Sets a single device transformation-related state.
old-location: direct3d9\idirect3ddevice9__settransform.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__settransform.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 25042e52-3212-5250-0bac-ab23f76aaeb1, IDirect3DDevice9 interface [Direct3D 9],SetTransform method, IDirect3DDevice9.SetTransform, IDirect3DDevice9::SetTransform, SetTransform, SetTransform method [Direct3D 9], SetTransform method [Direct3D 9],IDirect3DDevice9 interface, d3d9helper/IDirect3DDevice9::SetTransform, direct3d9.idirect3ddevice9__settransform
ms.topic: method
req.header: d3d9helper.h
req.include-header: D3D9.h
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
req.lib: D3D9.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D9.lib
 - D3D9.dll
api_name:
 - IDirect3DDevice9.SetTransform
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9::SetTransform


## -description


Sets a single device transformation-related state.


## -parameters




### -param State [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb172619(v=VS.85).aspx">D3DTRANSFORMSTATETYPE</a></b>

Device-state variable that is being modified. This parameter can be any member of the <a href="https://msdn.microsoft.com/en-us/library/Bb172619(v=VS.85).aspx">D3DTRANSFORMSTATETYPE</a> enumerated type, or the <a href="https://msdn.microsoft.com/en-us/library/Bb172623(v=VS.85).aspx">D3DTS_WORLDMATRIX</a> macro. 


### -param pMatrix [in]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/Bb172573(v=VS.85).aspx">D3DMATRIX</a>*</b>

Pointer to a <a href="https://msdn.microsoft.com/en-us/library/Bb172573(v=VS.85).aspx">D3DMATRIX</a> structure that modifies the current transformation. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. D3DERR_INVALIDCALL is returned if one of the arguments is invalid.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb172622(v=VS.85).aspx">D3DTS_WORLD</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb172623(v=VS.85).aspx">D3DTS_WORLDMATRIX</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb172624(v=VS.85).aspx">D3DTS_WORLDn</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174414(v=VS.85).aspx">IDirect3DDevice9::GetTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174454(v=VS.85).aspx">IDirect3DDevice9::SetRenderState</a>
 

 

