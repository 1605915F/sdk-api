---
UID: NF:directxpackedvector.XMStoreHalf4
title: XMStoreHalf4 function
author: windows-sdk-content
description: Stores an XMVECTOR in an XMHALF4.
old-location: dxmath\xmstorehalf4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.storing.XMStoreHalf4(XMHALF4@,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DirectX::PackedVector.XMStoreHalf4, XMStoreHalf4, XMStoreHalf4 method [DirectX Math Support APIs], dxmath.xmstorehalf4
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
 - XMStoreHalf4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMStoreHalf4 function


## -description


Stores an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> in an <a href="https://msdn.microsoft.com/en-us/library/Ee419664(v=VS.85).aspx">XMHALF4</a>.


## -parameters




### -param pDestination [out]

Address at which to store the data.


### -param V [in]

Vector containing the data to store.


## -returns



None.




## -remarks



This function takes a vector, converts the components into a half-precision format, and writes the results out to four half-precision floating-point values at the given address. The most significant component is written to the first two bytes of the address, the next most significant component is written to the next two bytes of the address, and so on.

The following pseudocode demonstrates the operation of the function.

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>pDestination-&gt;x = XMConvertFloatToHalf(V.x); // 2 bytes to address pDestination
pDestination-&gt;y = XMConvertFloatToHalf(V.y); // 2 bytes to address (uint8_t*)pDestination + 2
pDestination-&gt;z = XMConvertFloatToHalf(V.z); // 2 bytes to address (uint8_t*)pDestination + 4
pDestination-&gt;w = XMConvertFloatToHalf(V.w); // 2 bytes to address (uint8_t*)pDestination + 6</pre>
</td>
</tr>
</table></span></div>
<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/0e7b66bd-bdb0-956d-2962-b33ae52b3016">DirectXMath Library Vector Store Functions</a>
 

 

