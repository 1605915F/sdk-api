---
UID: NF:directxpackedvector.XMUSHORTN2.XMUSHORTN2(uint16_t,uint16_t)
title: XMUSHORTN2 function
author: windows-sdk-content
description: Initializes a new instance of XMUSHORTN2 from two uint16_t arguments.
old-location: dxmath\xmushortn2_ctor_2.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMUSHORTN2.#ctor(uint16_t,uint16_t)
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: XMUSHORTN2 constructor [DirectX Math Support APIs], XMUSHORTN2 constructor [DirectX Math Support APIs],XMUSHORTN2 structure, XMUSHORTN2 structure [DirectX Math Support APIs],XMUSHORTN2 constructor, XMUSHORTN2.XMUSHORTN2(uint16_t,uint16_t), dxmath.xmushortn2_ctor_2
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
 - XMUSHORTN2.XMUSHORTN2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- XMUSHORTN2
: 
---

# XMUSHORTN2 function


## -description


Initializes a new instance of <code>XMUSHORTN2</code> from two <code>uint16_t</code> arguments.
    

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/05f62462-2b6a-4d1b-bf83-9109a254839e">XMUSHORTN2</a> from two
	<code>uint16_t</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available under C++.
    </div><div> </div>

## -parameters




### -param _x

Value of the x-coordinate of the vector, the <b>x</b> member of the new
		    <code>XMUSHORTN2</code> instance.
		


### -param _y

Value of the y-coordinate of the vector, the <b>y</b> member of the new
		    <code>XMUSHORTN2</code> instance.
		


## -remarks



Input values are not normalized. The following pseudocode demonstrates the operation of
	    this constructor:
	

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMUSHORTN2 instance;

	instance.x = _x;
	instance.y = _y;


    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/05f62462-2b6a-4d1b-bf83-9109a254839e">XMUSHORTN2</a>



<a href="https://msdn.microsoft.com/89d5f55f-5603-4bc5-bf0b-4d6dae675ca3">XMUSHORTN2 Constructors</a>
 

 

