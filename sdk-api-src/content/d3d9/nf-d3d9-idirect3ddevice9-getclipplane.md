---
UID: NF:d3d9.IDirect3DDevice9.GetClipPlane
title: IDirect3DDevice9::GetClipPlane
author: windows-sdk-content
description: Retrieves the coefficients of a user-defined clipping plane for the device.
old-location: direct3d9\idirect3ddevice9__getclipplane.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__getclipplane.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 4ee4abff-6964-013c-ead5-e1d4da1fe84b, GetClipPlane, GetClipPlane method [Direct3D 9], GetClipPlane method [Direct3D 9],IDirect3DDevice9 interface, IDirect3DDevice9 interface [Direct3D 9],GetClipPlane method, IDirect3DDevice9.GetClipPlane, IDirect3DDevice9::GetClipPlane, d3d9helper/IDirect3DDevice9::GetClipPlane, direct3d9.idirect3ddevice9__getclipplane
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
 - IDirect3DDevice9.GetClipPlane
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9::GetClipPlane


## -description


Retrieves the coefficients of a user-defined clipping plane for the device.


## -parameters




### -param Index [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

Index of the clipping plane for which the plane equation coefficients are retrieved. 


### -param pPlane [out]

Type: <b>float*</b>

Pointer to a four-element array of values that represent the coefficients of the clipping plane in the form of the general plane equation. See Remarks. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value is D3DERR_INVALIDCALL. This error indicates that the value in Index exceeds the maximum clipping plane index supported by the device, or that the array at pPlane is not large enough to contain four floating-point values.




## -remarks



This method will not return device state for a device that is created using D3DCREATE_PUREDEVICE. If you want to use this method, you must create your device with any of the other values in <a href="https://msdn.microsoft.com/en-us/library/Bb172527(v=VS.85).aspx">D3DCREATE</a>."
    


The coefficients that this method reports take the form of the general plane equation. If the values in the array at pPlane were labeled A, B, C, and D in the order that they appear in the array, they would fit into the general plane equation so that Ax + By + Cz + Dw = 0. A point with homogeneous coordinates (x, y, z, w) is visible in the half space of the plane if Ax + By + Cz + Dw &gt;= 0. Points that exist on or behind the clipping plane are clipped from the scene.

The plane equation used by this method exists in world space and is set by a previous call to the <a href="https://msdn.microsoft.com/en-us/library/Bb174426(v=VS.85).aspx">IDirect3DDevice9::SetClipPlane</a> method.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174336(v=VS.85).aspx">IDirect3DDevice9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb174426(v=VS.85).aspx">IDirect3DDevice9::SetClipPlane</a>
 

 

