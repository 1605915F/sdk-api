---
UID: NF:d3d9helper.IDirect3DVolumeTexture9.UnlockBox
title: IDirect3DVolumeTexture9::UnlockBox
author: windows-sdk-content
description: Unlocks a box on a volume texture resource.
old-location: direct3d9\idirect3dvolumetexture9__unlockbox.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3dvolumetexture9__unlockbox.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 5b89d036-c0de-c93d-6c62-1b4072dc95c7, IDirect3DVolumeTexture9 interface [Direct3D 9],UnlockBox method, IDirect3DVolumeTexture9.UnlockBox, IDirect3DVolumeTexture9::UnlockBox, UnlockBox, UnlockBox method [Direct3D 9], UnlockBox method [Direct3D 9],IDirect3DVolumeTexture9 interface, d3d9helper/IDirect3DVolumeTexture9::UnlockBox, direct3d9.idirect3dvolumetexture9__unlockbox
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
 - IDirect3DVolumeTexture9.UnlockBox
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDirect3DVolumeTexture9::UnlockBox


## -description


Unlocks a box on a volume texture resource.


## -parameters




### -param Level [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Specifies the level of the volume texture resource to unlock. 


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value can be D3DERR_INVALIDCALL.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb205941(v=VS.85).aspx">IDirect3DVolumeTexture9</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb205945(v=VS.85).aspx">LockBox</a>
 

 

