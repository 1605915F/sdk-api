---
UID: NF:d3d9helper.IDirect3DDevice9.GetIndices
title: IDirect3DDevice9::GetIndices (d3d9helper.h)
author: windows-sdk-content
description: Retrieves index data.
old-location: direct3d9\idirect3ddevice9__getindices.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__getindices.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 137303d6-63b8-2f24-bcef-26fdda3c4a15, GetIndices, GetIndices method [Direct3D 9], GetIndices method [Direct3D 9],IDirect3DDevice9 interface, IDirect3DDevice9 interface [Direct3D 9],GetIndices method, IDirect3DDevice9.GetIndices, IDirect3DDevice9::GetIndices, d3d9helper/IDirect3DDevice9::GetIndices, direct3d9.idirect3ddevice9__getindices
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
 - IDirect3DDevice9.GetIndices
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDirect3DDevice9::GetIndices


## -description


Retrieves index data.


## -parameters




### -param ppIndexData [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb205865(v=VS.85).aspx">IDirect3DIndexBuffer9</a>**</b>

Address of a pointer to an <a href="https://msdn.microsoft.com/en-us/library/Bb205865(v=VS.85).aspx">IDirect3DIndexBuffer9</a> interface, representing the returned index data. 


#### - pBaseVertexIndex [out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

Pointer to a UINT value, holding the returned base value for vertex indices. This value is added to all indices prior to referencing vertex data, defining a starting position in the vertex streams. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value can be D3DERR_INVALIDCALL.




## -remarks



 Calling this method will increase the internal reference count on the <a href="https://msdn.microsoft.com/en-us/library/Bb205865(v=VS.85).aspx">IDirect3DIndexBuffer9</a> interface. Failure to call <a href="https://msdn.microsoft.com/4b494c6f-f0ee-4c35-ae45-ed956f40dc7a">IUnknown::Release</a> when finished using this <b>IDirect3DIndexBuffer9</b> interface results in a memory leak.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174369(v=VS.85).aspx">IDirect3DDevice9::DrawIndexedPrimitive</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174370(v=VS.85).aspx">IDirect3DDevice9::DrawIndexedPrimitiveUP</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174371(v=VS.85).aspx">IDirect3DDevice9::DrawPrimitive</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174372(v=VS.85).aspx">IDirect3DDevice9::DrawPrimitiveUP</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174435(v=VS.85).aspx">IDirect3DDevice9::SetIndices</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174595(v=VS.85).aspx">Index Buffers (Direct3D 9)</a>
 

 

