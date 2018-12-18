---
UID: NF:d3d9.IDirect3DSwapChain9.GetBackBuffer
title: IDirect3DSwapChain9::GetBackBuffer
author: windows-sdk-content
description: Retrieves a back buffer from the swap chain of the device.
old-location: direct3d9\idirect3dswapchain9__getbackbuffer.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3dswapchain9__getbackbuffer.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 138c5b9c-c0c2-7051-6dd4-c5933f8d32fa, GetBackBuffer, GetBackBuffer method [Direct3D 9], GetBackBuffer method [Direct3D 9],IDirect3DSwapChain9 interface, IDirect3DSwapChain9 interface [Direct3D 9],GetBackBuffer method, IDirect3DSwapChain9.GetBackBuffer, IDirect3DSwapChain9::GetBackBuffer, d3d9helper/IDirect3DSwapChain9::GetBackBuffer, direct3d9.idirect3dswapchain9__getbackbuffer
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
 - IDirect3DSwapChain9.GetBackBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DSwapChain9::GetBackBuffer


## -description


Retrieves a back buffer from the swap chain of the device.


## -parameters




### -param iBackBuffer [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Index of the back buffer object to return. Back buffers are numbered from 0 to the total number of back buffers - 1. A value of 0 returns the first back buffer, not the front buffer. The front buffer is not accessible through this method. Use <a href="https://msdn.microsoft.com/en-us/library/Bb205905(v=VS.85).aspx">IDirect3DSwapChain9::GetFrontBufferData</a> to retrieve a copy of the front buffer.


### -param Type [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb172506(v=VS.85).aspx">D3DBACKBUFFER_TYPE</a></b>

Stereo view is not supported in Direct3D 9, so the only valid value for this parameter is D3DBACKBUFFER_TYPE_MONO. 


### -param ppBackBuffer [out, retval]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a>**</b>

Address of a pointer to an <a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a> interface, representing the returned back buffer surface. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK.
 If BackBuffer exceeds or equals the total number of back buffers, then the function fails and returns D3DERR_INVALIDCALL.




## -remarks



Calling this method will increase the internal reference count on the <a href="https://msdn.microsoft.com/en-us/library/Bb205892(v=VS.85).aspx">IDirect3DSurface9</a> interface. Failure to call <a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">IUnknown::Release</a> when finished using this <b>IDirect3DSurface9</b> interface results in a memory leak. You must release any surfaces obtained through this method before releasing the swap chain it belongs to.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb205899(v=VS.85).aspx">IDirect3DSwapChain9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb205905(v=VS.85).aspx">IDirect3DSwapChain9::GetFrontBufferData</a>
 

 

