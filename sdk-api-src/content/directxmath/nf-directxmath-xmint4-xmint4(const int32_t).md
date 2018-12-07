---
UID: NF:directxmath.XMINT4.XMINT4(const int32_t)
title: XMINT4 function
author: windows-sdk-content
description: Initializes a new instance of XMINT4 from a four element int32_t array argument.
old-location: dxmath\xmint4_ctor_3.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMINT4.#ctor(const int32_t)
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: XMINT4 constructor [DirectX Math Support APIs], XMINT4 constructor [DirectX Math Support APIs],XMINT4 structure, XMINT4 structure [DirectX Math Support APIs],XMINT4 constructor, XMINT4.XMINT4(const int32_t), XMINT4.XMINT4(const int32_t*), dxmath.xmint4_ctor_3
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: directxmath.h
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
 - DirectXMath.h
api_name:
 - XMINT4.XMINT4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- XMINT4
: 
---

# XMINT4 function


## -description


Initializes a new instance of <code>XMINT4</code> from a four element <code>int32_t</code> array
	argument.
    

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/4562AF48-FC7E-4737-AB7B-7A76789DC70B">XMINT4</a> from a from
	a four element <code>int32_t</code> array argument.
<div class="alert"><b>Note</b>  This constructor is only available under C++.
    </div><div> </div>

## -parameters




### -param pArray

Four element <code>int32_t</code> array containing the values used to initialize the
		    four components of a new instance of <code>XMINT4</code>.
		


## -remarks



The following pseudocode demonstrates the operation of this constructor:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMINT4 instance;
	instance.x = pArray[0];
	instance.y = pArray[1];
	instance.z = pArray[2];
	instance.w = pArray[3];

    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/4562AF48-FC7E-4737-AB7B-7A76789DC70B">XMINT4</a>



<a href="https://msdn.microsoft.com/24ea5751-637d-4bd0-85f7-ce9895a10914">XMINT4 Constructors</a>
 

 

