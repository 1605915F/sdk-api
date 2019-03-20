---
UID: NF:d3d9.IDirect3DDevice9Ex.GetGPUThreadPriority
title: IDirect3DDevice9Ex::GetGPUThreadPriority (d3d9.h)
author: windows-sdk-content
description: Get the priority of the GPU thread.
old-location: direct3d9\idirect3ddevice9ex_getgputhreadpriority.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9ex_getgputhreadpriority.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetGPUThreadPriority, GetGPUThreadPriority method [Direct3D 9], GetGPUThreadPriority method [Direct3D 9],IDirect3DDevice9Ex interface, IDirect3DDevice9Ex interface [Direct3D 9],GetGPUThreadPriority method, IDirect3DDevice9Ex.GetGPUThreadPriority, IDirect3DDevice9Ex::GetGPUThreadPriority, d3d9/IDirect3DDevice9Ex::GetGPUThreadPriority, direct3d9.idirect3ddevice9ex_getgputhreadpriority, f7f920d1-5b01-e016-bbe8-663d05696c0e
ms.topic: method
req.header: d3d9.h
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
 - IDirect3DDevice9Ex.GetGPUThreadPriority
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9Ex::GetGPUThreadPriority


## -description


Get the priority of the GPU thread.


## -parameters




### -param pPriority

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">INT</a>*</b>

Current GPU priority. Valid values range from -7 to 7.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

Possible return values include: D3D_OK or D3DERR_DEVICEREMOVED (see <a href="https://msdn.microsoft.com/en-us/library/Bb172554(v=VS.85).aspx">D3DERR</a>).




## -remarks



Use <a href="https://msdn.microsoft.com/en-us/library/Bb174346(v=VS.85).aspx">IDirect3DDevice9Ex::SetGPUThreadPriority</a> to set the priority of a thread.

This method will retrieve the priority of the thread stored with the Direct3D device even if it was created with the <a href="https://msdn.microsoft.com/en-us/library/Bb172527(v=VS.85).aspx">D3DCREATE_PUREDEVICE</a> flag.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174337(v=VS.85).aspx">IDirect3DDevice9Ex</a>
 

 

