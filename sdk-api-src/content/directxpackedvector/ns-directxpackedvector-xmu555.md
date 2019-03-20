---
UID: NS:directxpackedvector.XMU555
title: XMU555 (directxpackedvector.h)
author: windows-sdk-content
description: A 4D vector with x-,y-, and z- components represented as 5 bit unsigned integer values, and the w-component as a 1 bit integer value.
old-location: dxmath\xmu555.htm
tech.root: dxmath
ms.assetid: T:Microsoft.directx_sdk.reference.XMU555
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMU555, XMU555 structure [DirectX Math Support APIs], directxpackedvector/XMU555, dxmath.xmu555
ms.topic: struct
req.header: directxpackedvector.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - DirectXPackedVector.h
api_name:
 - XMU555
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMU555 structure


## -description


A 4D vector with x-,y-, and z- components represented as 5 bit unsigned integer values, and
	the w-component as a 1 bit integer value.
    



For a list of additional functionality such as constructors and operators that are available
	using <code>XMU555</code> when you are programming in C++, see <a href="https://msdn.microsoft.com/en-us/library/Ee415438(v=VS.85).aspx">XMU555 Extensions</a>.


## -struct-fields




### -field x

 


### -field y

 


### -field z

 


### -field w

 


### -field v

Unsigned short representing the 4D vector.
			


### -field XMU555

TBD 


### -field operator uint16_t

TBD 


### -field operator=

TBD 




#### - w : 1

A 1-bit integer value in the range [0,31] describing the w-coordinate of
			    the vector.
			


#### - x : 5

Unsigned 5-bit integer value in the range [0,31] describing the
			    x-coordinate of the vector.
			


#### - y : 5

Unsigned 5-bit integer value in the range [0,31] describing the
			    y-coordinate of the vector.
			


#### - z : 5

Unsigned 5-bit integer value in the range [0,31] describing the
			    z-coordinate of the vector.
			


## -remarks



<code>XMU555</code> can be loaded into instances of <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1"> XMVECTOR</a> by
	    using <a href="https://msdn.microsoft.com/7023f2db-132d-475a-9b48-a676403567eb">XMLoadU555</a>.
	

Instances of <code>XMVECTOR</code> can be stored into an instance of <code>XMU555</code> with <a href="https://msdn.microsoft.com/en-us/library/Ee420374(v=VS.85).aspx">XMStoreU555</a>.
	

<b>Namespace:</b> Use DirectX::PackedVector

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/58acb05d-e79b-8f42-4cf4-76ae57929739">DirectXMath Library Structures</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415438(v=VS.85).aspx">XMU555 Extensions</a>
 

 

