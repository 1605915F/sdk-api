---
UID: NF:directxpackedvector.XMLoadU555
title: XMLoadU555 function
author: windows-sdk-content
description: Loads an XMU555 into an XMVECTOR.
old-location: dxmath\xmloadu555.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.loading.XMLoadU555(const XMU555)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DirectX::PackedVector.XMLoadU555, XMLoadU555, XMLoadU555 method [DirectX Math Support APIs], dxmath.xmloadu555
ms.topic: function
req.header: directxpackedvector.h
req.include-header: DirectXPackedVector.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: DirectX::PackedVector
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
 - directxpackedvector.inl
api_name:
 - XMLoadU555
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMLoadU555 function


## -description


Loads an <a href="https://msdn.microsoft.com/en-us/library/Ee420402(v=VS.85).aspx">XMU555</a> into an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a>.


## -parameters




### -param pSource [in]

Address of the <a href="https://msdn.microsoft.com/en-us/library/Ee420402(v=VS.85).aspx">XMU555</a> structure to load. 


## -returns



Returns an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> loaded with the data from the <i>pSource</i> parameter.




## -remarks



The following pseudocode demonstrates the operation of the function.

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
XMVECTOR vectorOut;

vectorOut.x = (float)pSource-&gt;x;
vectorOut.y = (float)pSource-&gt;y;
vectorOut.z = (float)pSource-&gt;z;
vectorOut.w = (float)pSource-&gt;w;

return vectorOut;
</pre>
</td>
</tr>
</table></span></div>
Note these are not normalized values. To convert to the RGBA 5/5/5/1 format, 
   you must scale the resulting vector by <code>(1.f/31.f, 1.f/31.f, 1.f/31.f, 1.f)</code>. 
   Also, you will probably need to swizzle the standard .x = RED, .y = GREEN, .z =
   BLUE, .w = ALPHA color vector's .x and .z value since the GPU format is BGR (not RGB).

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/3434ea7d-edc3-a8eb-3481-9e76ba724800">DirectXMath Library Vector Load Functions</a>
 

 

