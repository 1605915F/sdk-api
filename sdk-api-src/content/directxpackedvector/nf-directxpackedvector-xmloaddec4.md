---
UID: NF:directxpackedvector.XMLoadDec4
title: XMLoadDec4 function
author: windows-sdk-content
description: Loads an XMDEC4 into an XMVECTOR.
old-location: dxmath\xmloaddec4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.loading.XMLoadDec4(const XMDEC4)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DirectX::PackedVector.XMLoadDec4, XMLoadDec4, XMLoadDec4 method [DirectX Math Support APIs], dxmath.xmloaddec4
ms.topic: function
req.header: directxpackedvector.h
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
 - directxpackedvector.h
api_name:
 - XMLoadDec4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMLoadDec4 function


## -description


Loads an <a href="https://msdn.microsoft.com/en-us/library/Ee419431(v=VS.85).aspx">XMDEC4</a> into an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a>.


## -parameters




### -param pSource [in]

Address of the <a href="https://msdn.microsoft.com/en-us/library/Ee419431(v=VS.85).aspx">XMDEC4</a> structure to load. 


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
<pre>XMVECTOR vectorOut;

uint32_t Element;
static const uint32_t SignExtend[] = {0x00000000, 0xFFFFFC00};
static const uint32_t SignExtendW[] = {0x00000000, 0xFFFFFFFC};
	
Element = pSource-&gt;v &amp; 0x3FF;
vectorOut.x = (float)(int16_t)(Element | SignExtend[Element &gt;&gt; 9]);
Element = (pSource-&gt;v &gt;&gt; 10) &amp; 0x3FF;
vectorOut.y = (float)(int16_t)(Element | SignExtend[Element &gt;&gt; 9]);
Element = (pSource-&gt;v &gt;&gt; 20) &amp; 0x3FF;
vectorOut.z = (float)(int16_t)(Element | SignExtend[Element &gt;&gt; 9]);
Element = pSource-&gt;v &gt;&gt; 30;
vectorOut.w = (float)(int16_t)(Element | SignExtendW[Element &gt;&gt; 1]);

return vectorOut;</pre>
</td>
</tr>
</table></span></div>
<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/3434ea7d-edc3-a8eb-3481-9e76ba724800">DirectXMath Library Vector Load Functions</a>
 

 

