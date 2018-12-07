---
UID: NF:d3d9helper.IDirect3DDevice9.ColorFill
title: IDirect3DDevice9::ColorFill
author: windows-sdk-content
description: Allows an application to fill a rectangular area of a D3DPOOL_DEFAULT surface with a specified color.
old-location: direct3d9\idirect3ddevice9__colorfill.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__colorfill.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ColorFill, ColorFill method [Direct3D 9], ColorFill method [Direct3D 9],IDirect3DDevice9 interface, IDirect3DDevice9 interface [Direct3D 9],ColorFill method, IDirect3DDevice9.ColorFill, IDirect3DDevice9::ColorFill, b637fa24-0e80-8d43-dece-17fb81ac14e4, d3d9helper/IDirect3DDevice9::ColorFill, direct3d9.idirect3ddevice9__colorfill
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IDirect3DDevice9.ColorFill
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9::ColorFill


## -description


Allows an application to fill a rectangular area of a D3DPOOL_DEFAULT surface with a specified color.


## -parameters




### -param pSurface [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a>*</b>

Pointer to the surface to be filled.


### -param pRect [in]

Type: <b>const <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a>*</b>

Pointer to the source rectangle. Using <b>NULL</b> means that the entire surface will be filled.


### -param color [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb172518(v=VS.85).aspx">D3DCOLOR</a></b>

Color used for filling.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value can be
     D3DERR_INVALIDCALL.




## -remarks



This method can only be applied to a render target, a render-target texture surface, or an off-screen plain surface with a pool type of D3DPOOL_DEFAULT.

<b>IDirect3DDevice9::ColorFill</b> will work with all formats. However, when using a reference or software device, the only formats supported are D3DFMT_X1R5G5B5, D3DFMT_A1R5G5B5, D3DFMT_R5G6B5, D3DFMT_X8R8G8B8, D3DFMT_A8R8G8B8, D3DFMT_YUY2, D3DFMT_G8R8_G8B8, D3DFMT_UYVY, D3DFMT_R8G8_B8G8, D3DFMT_R16F, D3DFMT_G16R16F, D3DFMT_A16B16G16R16F, D3DFMT_R32F, D3DFMT_G32R32F, and D3DFMT_A32B32G32R32F.

When using a DirectX 7 or DirectX 8.x driver, the only YUV formats supported are D3DFMT_UYVY and D3DFMT_YUY2.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb172584(v=VS.85).aspx">D3DPOOL</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>
 

 

