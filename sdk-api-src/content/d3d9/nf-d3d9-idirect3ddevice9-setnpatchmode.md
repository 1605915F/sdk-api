---
UID: NF:d3d9.IDirect3DDevice9.SetNPatchMode
title: IDirect3DDevice9::SetNPatchMode
author: windows-sdk-content
description: Enable or disable N-patches.
old-location: direct3d9\idirect3ddevice9__setnpatchmode.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__setnpatchmode.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDirect3DDevice9 interface [Direct3D 9],SetNPatchMode method, IDirect3DDevice9.SetNPatchMode, IDirect3DDevice9::SetNPatchMode, SetNPatchMode, SetNPatchMode method [Direct3D 9], SetNPatchMode method [Direct3D 9],IDirect3DDevice9 interface, a1559401-14f3-1ada-91cb-f26fd6d19851, d3d9helper/IDirect3DDevice9::SetNPatchMode, direct3d9.idirect3ddevice9__setnpatchmode
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d9.h
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
 - IDirect3DDevice9.SetNPatchMode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9::SetNPatchMode


## -description


Enable or disable N-patches.


## -parameters




### -param nSegments [in]

Type: <b>float</b>

Specifies the number of subdivision segments. If the number of segments is less than 1.0, N-patches are disabled. The default value is 0.0. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK.






## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174395(v=VS.85).aspx">IDirect3DDevice9::GetNPatchMode</a>
 

 

