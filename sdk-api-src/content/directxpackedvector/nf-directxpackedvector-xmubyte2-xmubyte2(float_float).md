---
UID: NF:directxpackedvector.XMUBYTE2.XMUBYTE2(float,float)
title: XMUBYTE2::XMUBYTE2(float,float)
author: windows-sdk-content
description: Initializes a new instance of XMUBYTE2 from two float arguments.
old-location: dxmath\xmubyte2_ctor_4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMUBYTE2.#ctor(float,float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMUBYTE2, XMUBYTE2 constructor [DirectX Math Support APIs], XMUBYTE2 constructor [DirectX Math Support APIs],XMUBYTE2 structure, XMUBYTE2 structure [DirectX Math Support APIs],XMUBYTE2 constructor, XMUBYTE2.XMUBYTE2, XMUBYTE2.XMUBYTE2(float,float), XMUBYTE2::XMUBYTE2, XMUBYTE2::XMUBYTE2(float,float), dxmath.xmubyte2_ctor_4
ms.topic: method
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
 - DirectXPackedVector.h
api_name:
 - XMUBYTE2.XMUBYTE2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMUBYTE2::XMUBYTE2(float,float)


## -description


Initializes a new instance of <code>XMUBYTE2</code> from two <code>float</code> arguments.

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/en-us/library/Hh404719(v=VS.85).aspx">XMUBYTE2</a> from two <code>float</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available with C++.</div><div> </div>

## -parameters




### -param _x

Value of the x-coordinate of the vector, the <b>x</b> member of the new <code>XMUBYTE2</code> instance.


### -param _y

Value of the y-coordinate of the vector, the <b>y</b> member of the new <code>XMUBYTE2</code> instance.


## -remarks



The magnitude of each argument to the constructor will be clamped to the range supported by an 8-bit signed integer [0,
   255.0].

The following pseudocode demonstrates the operation of this constructor:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMUBYTE2 instance;

	instance.x = (uint8_t)min( max( _x, 0.0 ), 255.0 );
	instance.y = (uint8_t)min( max( _y, 0.0 ), 255.0 );
    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Hh404719(v=VS.85).aspx">XMUBYTE2</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449522(v=VS.85).aspx">XMUBYTE2 Constructors</a>
 

 

