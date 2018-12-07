---
UID: NF:directxpackedvector.XMStoreDec4
title: XMStoreDec4 function
author: windows-sdk-content
description: Stores an XMVECTOR in an XMDEC4.
old-location: dxmath\xmstoredec4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.storing.XMStoreDec4(XMDEC4@,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DirectX::PackedVector.XMStoreDec4, XMStoreDec4, XMStoreDec4 method [DirectX Math Support APIs], dxmath.xmstoredec4
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - XMStoreDec4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMStoreDec4 function


## -description


Stores an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> in an <a href="https://msdn.microsoft.com/en-us/library/Ee419431(v=VS.85).aspx">XMDEC4</a>.


## -parameters




### -param pDestination [out]

Address at which to store the data.


### -param V [in]

Vector containing the data to store.


## -returns



None.




## -remarks



The following pseudocode demonstrates the operation of the function.

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>XMVECTOR N;	
static const XMVECTOR  Min = {-511.0f, -511.0f, -511.0f, -1.0f};
static const XMVECTOR  Max = {511.0f, 511.0f, 511.0f, 1.0f};

N = XMVectorClamp(V, Min, Max);

pDestination-&gt;v = ((int32_t)N.v[3] &lt;&lt; 30) |
                  (((int32_t)N.v[2] &amp; 0x3FF) &lt;&lt; 20) |
                  (((int32_t)N.v[1] &amp; 0x3FF) &lt;&lt; 10) |
                  (((int32_t)N.v[0] &amp; 0x3FF));</pre>
</td>
</tr>
</table></span></div>
<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/0e7b66bd-bdb0-956d-2962-b33ae52b3016">DirectXMath Library Vector Store Functions</a>
 

 

