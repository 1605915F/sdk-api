---
UID: NF:d3d9.IDirect3DDevice9.GetFVF
title: IDirect3DDevice9::GetFVF
author: windows-sdk-content
description: Gets the fixed vertex function declaration.
old-location: direct3d9\idirect3ddevice9__getfvf.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__getfvf.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 951f24cf-f72e-7ab4-8fde-fbe96bc36c7a, GetFVF, GetFVF method [Direct3D 9], GetFVF method [Direct3D 9],IDirect3DDevice9 interface, IDirect3DDevice9 interface [Direct3D 9],GetFVF method, IDirect3DDevice9.GetFVF, IDirect3DDevice9::GetFVF, d3d9helper/IDirect3DDevice9::GetFVF, direct3d9.idirect3ddevice9__getfvf
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
 - IDirect3DDevice9.GetFVF
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9::GetFVF


## -description


Gets the fixed vertex function declaration.


## -parameters




### -param pFVF [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a>*</b>

A DWORD pointer to the fixed function vertex type. For more information, see <a href="https://msdn.microsoft.com/en-us/library/Bb172559(v=VS.85).aspx">D3DFVF</a>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value can be
     D3DERR_INVALIDCALL.




## -remarks



The fixed vertex function declaration is a set of FVF flags that determine how vertices processed by the fixed function pipeline will be used.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174433(v=VS.85).aspx">IDirect3DDevice9::SetFVF</a>
 

 

