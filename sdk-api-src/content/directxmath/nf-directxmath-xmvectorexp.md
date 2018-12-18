---
UID: NF:directxmath.XMVectorExp
title: XMVectorExp function
author: windows-sdk-content
description: Computes two raised to the power for each component.Note  This function is a compatibility alias for XMVectorExp2 for existing Windows 8 code. This function is deprecated for Windows 8.1. Don't use it and instead use XMVectorExp2 or XMVectorExpE.  .
old-location: dxmath\xmvectorexp.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.transcendental.XMVectorExp(XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorExp, XMVectorExp, XMVectorExp method [DirectX Math Support APIs], dxmath.xmvectorexp
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
 - XMVectorExp
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorExp function


## -description


Computes two raised to the power for each component.<div class="alert"><b>Note</b>  This function is a compatibility alias for <a href="https://msdn.microsoft.com/1B04528B-532B-4555-B027-D5EC33DD9843">XMVectorExp2</a> for existing Windows 8 code. This function is deprecated for Windows 8.1. Don't use it and instead use <b>XMVectorExp2</b> or <a href="https://msdn.microsoft.com/C4A5E4E0-56CC-46E3-87C5-CA99EF512B11">XMVectorExpE</a>.
</div>
<div> </div>



## -parameters




### -param V [in]

Vector used for the exponents of base two.


## -returns



Returns a vector whose components are two raised to the power of the corresponding component of <i>V</i>.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/aae12d4a-7758-83df-5376-99d5d94a28c4">Transcendental Vector Functions</a>
 

 

