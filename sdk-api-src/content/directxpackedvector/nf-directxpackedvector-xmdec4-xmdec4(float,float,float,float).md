---
UID: NF:directxpackedvector.XMDEC4.XMDEC4(float,float,float,float)
title: XMDEC4 function
author: windows-sdk-content
description: Initializes a new instance of XMDEC4 from four float arguments.
old-location: dxmath\xmdec4_ctor_3.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMDEC4.#ctor(float,float,float,float)
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: XMDEC4 constructor [DirectX Math Support APIs], XMDEC4 constructor [DirectX Math Support APIs],XMDEC4 structure, XMDEC4 structure [DirectX Math Support APIs],XMDEC4 constructor, XMDEC4.XMDEC4(float,float,float,float), dxmath.xmdec4_ctor_3
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
 - XMDEC4.XMDEC4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- XMDEC4
: 
---

# XMDEC4 function


## -description


Initializes a new instance of <code>XMDEC4</code> from four <code>float</code> arguments.
    

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/a52fa5e4-ee45-4256-a06a-6984d63b5578">XMDEC4 </a> from four
	<code>float</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available under C++.
    </div><div> </div>

## -parameters




### -param _x

Value of the x-coordinate of the vector, the <b>x</b> member of the new
		    <code>XMDEC4</code> instance.
		

The magnitude of this argument will be clamped to a range of [-511.0,
		    511.0].
		


### -param _y

Value of the y-coordinate of the vector, the <b>y</b> member of the new
		    <code>XMDEC4</code> instance.
		

The magnitude of this argument will be clamped to a range of [-511.0,
		    511.0].
		


### -param _z

Value of the z-coordinate of the vector, the <b>z</b> member of the new
		    <code>XMDEC4</code> instance.
		

The magnitude of this argument will be clamped to a range of [-511.0,
		    511.0].
		


### -param _w

Value of the w-coordinate of the vector, the <b>w</b> member of the new
		    <code>XMDEC4</code> instance.
		

The magnitude of this argument will be clamped to a range of [-1.0,
		    1.0].
		


## -remarks



The following pseudocode demonstrates the operation of this constructor, which takes
	    advantage of the <code>union</code> of the four components of the <code>XMDEC4</code> vector
	    with an instance of <code>uint32_t</code> in the definition of the structure:
	

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMDEC4 instance;
	_x1=min( max( _x, -511.0 ), 511.0 );
	_y1=min( max( _y, -511.0 ), 511.0 );
	_z1=min( max( _z, -511.0 ), 511.0 );
	_w1=min( max( _w, -1.0 ), 1.0 );


	instance.v =  ( (int32_t)_w1 &lt;&lt; 30) |
                      (((int32_t)_z1 &amp; 0x3FF) &lt;&lt; 20) |
                      (((int32_t)_y1 &amp; 0x3FF) &lt;&lt; 10) |
                      (((int32_t)_x1 &amp; 0x3FF));
      </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/a52fa5e4-ee45-4256-a06a-6984d63b5578">XMDEC4</a>



<a href="https://msdn.microsoft.com/e8ca8689-c946-4fef-a211-6c3737cc88aa">XMDEC4 Constructors</a>
 

 

