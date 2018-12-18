---
UID: NF:directxmath.XMVectorEqualIntR
title: XMVectorEqualIntR function
author: windows-sdk-content
description: Performs a per-component test for equality of two vectors, treating each component as an unsigned integer. In addition, this function sets a comparison value that can be examined using functions such as XMComparisonAllTrue.
old-location: dxmath\xmvectorequalintr.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.comparison.XMVectorEqualIntR(uint32_t@,XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorEqualIntR, XMVectorEqualIntR, XMVectorEqualIntR method [DirectX Math Support APIs], dxmath.xmvectorequalintr
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
 - XMVectorEqualIntR
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorEqualIntR function


## -description


Performs a per-component test for equality of two vectors, treating each component as an unsigned integer. In addition, this function sets a comparison value that can be examined using functions such as <a href="https://msdn.microsoft.com/en-us/library/Hh437887(v=VS.85).aspx">XMComparisonAllTrue</a>.


## -parameters




### -param pCR [out]

Pointer to a <b>uint32_t</b> comparison value that can be examined using functions such as <a href="https://msdn.microsoft.com/en-us/library/Hh437887(v=VS.85).aspx">XMComparisonAllTrue</a>. The <code>XMComparisonXXXX</code> functions may be used to further test the number of components that passed the comparison.


### -param V

TBD


### -param V2 [in]

Second vector to compare.


#### - V1 [in]

First vector to compare.


## -returns



Returns a vector containing the results of each component test.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/8caad40f-ab8e-db2f-da11-18f3d3ccf6ef">Vector Comparison Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee421013(v=VS.85).aspx">XMVectorEqual</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee421014(v=VS.85).aspx">XMVectorEqualInt</a>
 

 

