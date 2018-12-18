---
UID: NF:directxmath.XMVector2AngleBetweenVectors
title: XMVector2AngleBetweenVectors function
author: windows-sdk-content
description: Computes the radian angle between two 2D vectors.
old-location: dxmath\xmvector2anglebetweenvectors.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.geometric.XMVector2AngleBetweenVectors(XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVector2AngleBetweenVectors, XMVector2AngleBetweenVectors, XMVector2AngleBetweenVectors method [DirectX Math Support APIs], dxmath.xmvector2anglebetweenvectors
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
 - XMVector2AngleBetweenVectors
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVector2AngleBetweenVectors function


## -description


Computes the radian angle between two 2D vectors.


## -parameters




### -param V1 [in]

2D vector.


### -param V2 [in]

2D vector.


## -returns



Returns a vector. The radian angle between <i>V1</i> and <i>V2</i> is replicated to each of the components.




## -remarks



If V1 and V2 are normalized 2D vectors, it is faster to use <a href="https://msdn.microsoft.com/en-us/library/Ee420744(v=VS.85).aspx">XMVector2AngleBetweenNormals</a>.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/a17cdad7-4fbe-bf83-472f-1b99603b7fec">DirectXMath Library 2D Vector Geometric Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee420744(v=VS.85).aspx">XMVector2AngleBetweenNormals</a>
 

 

