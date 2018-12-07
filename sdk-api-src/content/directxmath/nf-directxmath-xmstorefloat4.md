---
UID: NF:directxmath.XMStoreFloat4
title: XMStoreFloat4 function
author: windows-sdk-content
description: Stores an XMVECTOR in an XMFLOAT4.
old-location: dxmath\xmstorefloat4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.storing.XMStoreFloat4(XMFLOAT4@,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMStoreFloat4, XMStoreFloat4, XMStoreFloat4 method [DirectX Math Support APIs], dxmath.xmstorefloat4
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: directxmath.h
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
req.namespace: Use DirectX.
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - DirectXMath.h
api_name:
 - XMStoreFloat4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMStoreFloat4 function


## -description


Stores an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> in an <a href="https://msdn.microsoft.com/2af4929b-9e44-4229-916e-d7d8eae07306">XMFLOAT4</a>.


## -parameters




### -param pDestination [out]

Address at which to store the data.


### -param V [in]

Vector containing the data to store.


## -returns



None.




## -remarks



This function takes a vector and writes the components out to four single-precision floating-point values at the given address. The most significant component is written to the first four bytes of the address, the next most significant component is written to the next four bytes, and so on.

The following pseudocode demonstrates the operation of the function.


```
pDestination->x = V.x; // 4 bytes to address pDestination
pDestination->y = V.y; // 4 bytes to address (uint8_t*)pDestination + 4
pDestination->z = V.z; // 4 bytes to address (uint8_t*)pDestination + 8
pDestination->w = V.w; // 4 bytes to address (uint8_t*)pDestination + 12
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/0e7b66bd-bdb0-956d-2962-b33ae52b3016">DirectXMath Library Vector Store Functions</a>
 

 

