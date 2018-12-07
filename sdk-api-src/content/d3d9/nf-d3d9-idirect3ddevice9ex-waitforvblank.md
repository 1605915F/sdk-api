---
UID: NF:d3d9.IDirect3DDevice9Ex.WaitForVBlank
title: IDirect3DDevice9Ex::WaitForVBlank
author: windows-sdk-content
description: Suspend execution of the calling thread until the next vertical blank signal.
old-location: direct3d9\idirect3ddevice9ex_waitforvblank.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9ex_waitforvblank.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 0c60116d-ada5-3625-26f3-44646e467dd6, IDirect3DDevice9Ex interface [Direct3D 9],WaitForVBlank method, IDirect3DDevice9Ex.WaitForVBlank, IDirect3DDevice9Ex::WaitForVBlank, WaitForVBlank, WaitForVBlank method [Direct3D 9], WaitForVBlank method [Direct3D 9],IDirect3DDevice9Ex interface, d3d9/IDirect3DDevice9Ex::WaitForVBlank, direct3d9.idirect3ddevice9ex_waitforvblank
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IDirect3DDevice9Ex.WaitForVBlank
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DDevice9Ex::WaitForVBlank


## -description


Suspend execution of the calling thread until the next vertical blank signal.


## -parameters




### -param iSwapChain [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Swap chain index. This is an optional, zero-based index used to specify a swap chain on a multihead card.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

This method will always return D3D_OK.




## -remarks



This method allows applications to efficiently throttle their frame rate to that of the monitor associated with the device. Following a vertical blank, the amount of time it takes for the thread to wake up is typically very short.

In some scenarios the hardware may stop generating vertical blank signals when nothing is being displayed on the monitor. In this case, the method will wait approximately 100ms and return with D3D_OK.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb174337(v=VS.85).aspx">IDirect3DDevice9Ex</a>
 

 

