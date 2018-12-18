---
UID: NF:d3d9helper.IDirect3DDevice9.CreateOffscreenPlainSurface
title: IDirect3DDevice9::CreateOffscreenPlainSurface
author: windows-sdk-content
description: Create an off-screen surface.
old-location: direct3d9\idirect3ddevice9__createoffscreenplainsurface.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__createoffscreenplainsurface.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateOffscreenPlainSurface, CreateOffscreenPlainSurface method [Direct3D 9], CreateOffscreenPlainSurface method [Direct3D 9],IDirect3DDevice9 interface, IDirect3DDevice9 interface [Direct3D 9],CreateOffscreenPlainSurface method, IDirect3DDevice9.CreateOffscreenPlainSurface, IDirect3DDevice9::CreateOffscreenPlainSurface, d3d9helper/IDirect3DDevice9::CreateOffscreenPlainSurface, direct3d9.idirect3ddevice9__createoffscreenplainsurface, f714d72c-a698-e4b2-14cb-1951e38364a8
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
 - IDirect3DDevice9.CreateOffscreenPlainSurface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9::CreateOffscreenPlainSurface


## -description


Create an off-screen surface.


## -parameters




### -param Width [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Width of the surface.


### -param Height [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Height of the surface.


### -param Format [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb172558(v=VS.85).aspx">D3DFORMAT</a></b>

Format of the surface. See <a href="https://msdn.microsoft.com/en-us/library/Bb172558(v=VS.85).aspx">D3DFORMAT</a>. 


### -param Pool [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb172584(v=VS.85).aspx">D3DPOOL</a></b>

Surface pool type. See <a href="https://msdn.microsoft.com/en-us/library/Bb172584(v=VS.85).aspx">D3DPOOL</a>.


### -param ppSurface [out, retval]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a>**</b>

Pointer to the <a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a>  interface created.


### -param pSharedHandle [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HANDLE</a>*</b>

Reserved. Set this parameter to <b>NULL</b>. This parameter can be used in Direct3D 9 for Windows Vista to <a href="https://msdn.microsoft.com/en-us/library/Bb219800(v=VS.85).aspx">share resources</a>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value can be the following:
     D3DERR_INVALIDCALL.




## -remarks



D3DPOOL_SCRATCH will return a surface that has identical characteristics to a surface created by the DirectX 8.x method CreateImageSurface.

D3DPOOL_DEFAULT is the appropriate pool for use with the <a href="https://msdn.microsoft.com/en-us/library/Bb174471(v=VS.85).aspx">IDirect3DDevice9::StretchRect</a> and <a href="https://msdn.microsoft.com/en-us/library/Bb174353(v=VS.85).aspx">IDirect3DDevice9::ColorFill</a>.

D3DPOOL_MANAGED is not allowed when creating an offscreen plain surface. For more information about memory pools, see <a href="https://msdn.microsoft.com/en-us/library/Bb172584(v=VS.85).aspx">D3DPOOL</a>.

Off-screen plain surfaces are always lockable, regardless of their pool types.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>
 

 

