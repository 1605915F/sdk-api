---
UID: NF:d3d9.IDirect3DDevice9.GetBackBuffer
title: IDirect3DDevice9::GetBackBuffer
author: windows-sdk-content
description: Retrieves a back buffer from the device's swap chain.
old-location: direct3d9\idirect3ddevice9__getbackbuffer.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__getbackbuffer.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetBackBuffer, GetBackBuffer method [Direct3D 9], GetBackBuffer method [Direct3D 9],IDirect3DDevice9 interface, IDirect3DDevice9 interface [Direct3D 9],GetBackBuffer method, IDirect3DDevice9.GetBackBuffer, IDirect3DDevice9::GetBackBuffer, b04301e3-b180-4cfd-097e-28f74fd7b3a9, d3d9helper/IDirect3DDevice9::GetBackBuffer, direct3d9.idirect3ddevice9__getbackbuffer
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
 - IDirect3DDevice9.GetBackBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9::GetBackBuffer


## -description


Retrieves a back buffer from the device's swap chain.


## -parameters




### -param iSwapChain [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

An unsigned integer specifying the swap chain.


### -param iBackBuffer [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index of the back buffer object to return. Back buffers are numbered from 0 to the total number of back buffers minus one. A value of 0 returns the first back buffer, not the front buffer. The front buffer is not accessible through this method. Use <a href="https://msdn.microsoft.com/en-us/library/Bb174388(v=VS.85).aspx">IDirect3DDevice9::GetFrontBufferData</a> to retrieve a copy of the front buffer.


### -param Type [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb172506(v=VS.85).aspx">D3DBACKBUFFER_TYPE</a></b>

Stereo view is not supported in Direct3D 9, so the only valid value for this parameter is D3DBACKBUFFER_TYPE_MONO. 


### -param ppBackBuffer [out, retval]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a>**</b>

Address of a pointer to an <a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a> interface, representing the returned back buffer surface. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If BackBuffer equals or exceeds the total number of back buffers, then the function fails and returns D3DERR_INVALIDCALL.




## -remarks



Calling this method will increase the internal reference count on the <a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a> interface. Failure to call <a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">IUnknown::Release</a> when finished using this <b>IDirect3DSurface9</b> interface results in a memory leak.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174388(v=VS.85).aspx">IDirect3DDevice9::GetFrontBufferData</a>
 

 

