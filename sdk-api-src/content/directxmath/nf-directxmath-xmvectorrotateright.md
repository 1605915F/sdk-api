---
UID: NF:directxmath.XMVectorRotateRight
title: XMVectorRotateRight function
author: windows-sdk-content
description: Rotates the vector right by a given number of 32-bit elements.
old-location: dxmath\xmvectorrotateright.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.component-wise.XMVectorRotateRight(XMVECTOR,uint32_t)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorRotateRight, XMVectorRotateRight, XMVectorRotateRight method [DirectX Math Support APIs], dxmath.xmvectorrotateright
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
 - XMVectorRotateRight
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorRotateRight function


## -description


Rotates the vector right by a given number of 32-bit elements.


## -parameters




### -param V [in]

Vector to rotate right.


### -param Elements [in]

Number of 32-bit elements by which to rotate <i>V</i> right. This parameter must be 0, 1, 2, or 3.


## -returns



Returns the rotated <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a>.




## -remarks



The following code demonstrates how this function may be used.


```
XMVECTOR v = XMVectorSet( 10.0f, 20.0f, 30.0f, 40.0f );
XMVECTOR result = XMVectorRotateRight( v, 1 );
```


The rotated vector (<i>result</i>) will be &lt;40.0f, 10.0f, 20.0f, 30.0f&gt;.

In the case of a constant rotate value, it is more efficient to use the template form of <a href="https://msdn.microsoft.com/en-us/library/Hh855946(v=VS.85).aspx">XMVectorRotateRight</a>:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
template<uint32_t Elements>
    XMVECTOR XMVectorRotateRight(FXMVECTOR V)
   </pre>
</td>
</tr>
</table></span></div>


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/f5464614-f6bb-427d-5488-3ba0fd4c6e8d">Component-Wise Vector Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh855956(v=VS.85).aspx">XMVectorPermute</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh404806(v=VS.85).aspx">XMVectorRotateLeft</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh404823(v=VS.85).aspx">XMVectorShiftLeft</a>
 

 

