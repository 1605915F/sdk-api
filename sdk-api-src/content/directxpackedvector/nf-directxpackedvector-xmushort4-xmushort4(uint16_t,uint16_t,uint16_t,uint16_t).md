---
UID: NF:directxpackedvector.XMUSHORT4.XMUSHORT4(uint16_t,uint16_t,uint16_t,uint16_t)
title: XMUSHORT4 function
author: windows-sdk-content
description: Initializes a new instance of XMUSHORT4 from four uint16_t arguments.
old-location: dxmath\xmushort4_ctor_2.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMUSHORT4.#ctor(uint16_t,uint16_t,uint16_t,uint16_t)
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: XMUSHORT4 constructor [DirectX Math Support APIs], XMUSHORT4 constructor [DirectX Math Support APIs],XMUSHORT4 structure, XMUSHORT4 structure [DirectX Math Support APIs],XMUSHORT4 constructor, XMUSHORT4.XMUSHORT4(uint16_t,uint16_t,uint16_t,uint16_t), dxmath.xmushort4_ctor_2
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
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
 - XMUSHORT4.XMUSHORT4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- XMUSHORT4
: 
---

# XMUSHORT4 function


## -description


Initializes a new instance of <code>XMUSHORT4</code> from four <code>uint16_t</code> arguments.
    

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/313a6fd0-d681-453a-8390-e0dafa309064">XMUSHORT4</a> from a
	four <code>uint16_t</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available under C++.
    </div><div> </div>

## -parameters




### -param _x

Value of the x-coordinate of the vector, the <b>x</b> member of the new
		    <code>XMUSHORT4</code> instance.
		


### -param _y

Value of the y-coordinate of the vector, the <b>y</b> member of the new
		    <code>XMUSHORT4</code> instance.
		


### -param _z

Value of the z-coordinate of the vector, the <b>z</b> member of the new
		    <code>XMUSHORT4</code> instance.
		


### -param _w

Value of the w-coordinate of the vector, the <b>w</b> member of the new
		    <code>XMUSHORT4</code> instance.
		


## -remarks



The following pseudocode demonstrates the operation of this constructor:
	

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMUSHORT4 instance;

	instance.x = _x;
	instance.y = _y;
	instance.z = _z;
	instance.w = _w;

    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/313a6fd0-d681-453a-8390-e0dafa309064">XMUSHORT4</a>



<a href="https://msdn.microsoft.com/7f822c43-69a6-442a-bb30-adfafe5399ff">XMUSHORT4 Constructors</a>
 

 

