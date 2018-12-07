---
UID: NF:directxmath.XMVectorCos
title: XMVectorCos function
author: windows-sdk-content
description: Computes the cosine of each component of an XMVECTOR.
old-location: dxmath\xmvectorcos.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.transcendental.XMVectorCos(XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorCos, XMVectorCos, XMVectorCos method [DirectX Math Support APIs], dxmath.xmvectorcos
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: directxmath.h
req.include-header: DirectXMath.h
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
 - directxmathvector.inl
api_name:
 - XMVectorCos
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorCos function


## -description


Computes the cosine of each component of an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a>.


## -parameters




### -param V [in]

Vector for which to compute the cosine.


## -returns



Returns a vector. Each component is the cosine of the corresponding component of <i>V</i>.




## -remarks



This function uses a 10-degree minimax approximation.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/aae12d4a-7758-83df-5376-99d5d94a28c4">Transcendental Vector Functions</a>



<a href="https://msdn.microsoft.com/1d78bd1e-de56-4e60-817d-8ad10af86471">XMVectorACos</a>



<a href="https://msdn.microsoft.com/162da582-d82f-4c48-995f-3c3750ea8df1">XMVectorACosEst</a>



<a href="https://msdn.microsoft.com/8c7ee39d-76b5-476a-bfa0-ab77594e114c">XMVectorCosEst</a>
 

 

