---
UID: NF:directxmath.XMVectorInBoundsR
title: XMVectorInBoundsR function (directxmath.h)
author: windows-sdk-content
description: Tests whether the components of a given vector are within certain bounds and sets a comparison value that can be examined using functions such as XMComparisonAllTrue.
old-location: dxmath\xmvectorinboundsr.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.geometric.XMVectorInBoundsR(uint32_t@,XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Use DirectX..XMVectorInBoundsR, XMVectorInBoundsR, XMVectorInBoundsR method [DirectX Math Support APIs], dxmath.xmvectorinboundsr
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
 - XMVectorInBoundsR
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorInBoundsR function


## -description


Tests whether the components of a given vector are within certain bounds and sets a comparison value that can be examined using functions such as <a href="https://msdn.microsoft.com/en-us/library/Hh437887(v=VS.85).aspx">XMComparisonAllTrue</a>.


## -parameters




### -param pCR [out]

Pointer to a <b>uint32_t</b> comparison value that can be examined using functions such as <a href="https://msdn.microsoft.com/en-us/library/Hh437886(v=VS.85).aspx">XMComparisonAllInBounds</a>. The <code>XMComparisonXXXX</code> functions may be used to further test the number of components that passed the comparison.


### -param V [in]

Vector to test.


### -param Bounds [in]

Vector that determines the bounds.


## -returns



Returns a vector containing the results of each component test.




## -remarks



The following pseudocode demonstrates the comparison operation of the function:


```
XMVECTOR Control;

Control.x = (V.x <= Bounds.x && V.x >= -Bounds.x) ? 0xFFFFFFFF : 0;
Control.y = (V.y <= Bounds.y && V.y >= -Bounds.y) ? 0xFFFFFFFF : 0;
Control.z = (V.z <= Bounds.z && V.z >= -Bounds.z) ? 0xFFFFFFFF : 0;
Control.w = (V.w <= Bounds.w && V.w >= -Bounds.w) ? 0xFFFFFFFF : 0;

return Control;
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/7c941454-7410-f3fb-d750-9007f672ed8c">Geometric Vector Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee421166(v=VS.85).aspx">XMVectorInBounds</a>
 

 

