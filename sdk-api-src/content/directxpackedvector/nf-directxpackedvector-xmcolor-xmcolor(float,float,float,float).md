---
UID: NF:directxpackedvector.XMCOLOR.XMCOLOR(float,float,float,float)
title: XMCOLOR function
author: windows-sdk-content
description: Initializes a new instance of XMCOLOR from four float arguments.
old-location: dxmath\xmcolor_ctor_3.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMCOLOR.#ctor(float,float,float,float)
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: XMCOLOR constructor [DirectX Math Support APIs], XMCOLOR constructor [DirectX Math Support APIs],XMCOLOR structure, XMCOLOR structure [DirectX Math Support APIs],XMCOLOR constructor, XMCOLOR.XMCOLOR(float,float,float,float), dxmath.xmcolor_ctor_3
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
 - XMCOLOR.XMCOLOR
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- XMCOLOR
: 
---

# XMCOLOR function


## -description


Initializes a new instance of <code>XMCOLOR</code> from four <code>float</code> arguments.
    

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/B799AA06-C51B-440A-93AD-3D3334449E27">XMCOLOR </a> from four
	<code>float</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available under C++.
    </div><div> </div>

## -parameters




### -param _r

Normalized value for the <i>red</i> channel of a 32-bit ARGB color
		    stored in the new instance of <code>XMCOLOR</code>. The value of this argument
		    should be in the range [0.0 - 1.0].
		    


### -param _g

Normalized value for the <i>green</i> channel of a 32-bit ARGB
		    color stored in the new instance of <code>XMCOLOR</code>. The value of this
		    argument should be in the range [0.0 - 1.0].
		    


### -param _b

Normalized value for the <i>blue</i> channel of a 32-bit ARGB
		    color stored in the new instance of <code>XMCOLOR</code>. The value of this
		    argument should be in the range [0.0 - 1.0].
		    


### -param _a

Normalized value for the <i>alpha</i> channel of a 32-bit ARGB
		    color stored in the new instance of <code>XMCOLOR</code>. The value of this
		    argument should be in the range [0.0 - 1.0].
		    


## -remarks



During the instantiation of an instance of <code>XMCOLOR</code>, all input arguments to
	    this constructor are clamped to a range of [0.0, 1.0], multiplied by <code>255.0f</code>,
	    as well as rounded, and before being stored in the appropriate structure member.
	  

The following pseudocode demonstrates the operation of this constructor, which takes
	    advantage of the <code>union</code> of the four components of the <code>XMCOLOR</code>vector with an instance of <code>uint32_t</code> in the definition of the structure:
	  

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
        XMCOLOR instance;        
	_a1 = min( max( _a, 0.0 ), 1.0 );
	_r1 = min( max( _r, 0.0 ), 1.0 );
	_g1 = min( max( _g, 0.0 ), 1.0 );
	_b1 = min( max( _b, 0.0 ), 1.0 );

	_a1 = round ( _a1 * 255.0f );
	_r1 = round ( _r1 * 255.0f );
	_g1 = round ( _g1 * 255.0f );
	_b1 = round ( _b1 * 255.0f );

	instance.v =  ( (uint32_t)_a1  &lt;&lt; 24) |
                      ( (uint32_t)_r1  &lt;&lt; 16) |
                      ( (uint32_t)_b1  &lt;&lt;  8) |
                      ( (uint32_t)_b1 );
    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/B799AA06-C51B-440A-93AD-3D3334449E27">XMCOLOR</a>



<a href="https://msdn.microsoft.com/9d700016-8a5c-4699-b9cb-f9e91296a2a7">XMCOLOR Constructors</a>
 

 

