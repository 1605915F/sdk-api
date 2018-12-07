---
UID: NF:directxmath.XMINT3.XMINT3(const int32_t)
title: XMINT3 function
author: windows-sdk-content
description: Initializes a new instance of XMINT3 from a three element int32_t array argument.
old-location: dxmath\xmint3_ctor_3.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMINT3.#ctor(const int32_t)
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: XMINT3 constructor [DirectX Math Support APIs], XMINT3 constructor [DirectX Math Support APIs],XMINT3 structure, XMINT3 structure [DirectX Math Support APIs],XMINT3 constructor, XMINT3.XMINT3(const int32_t), XMINT3.XMINT3(const int32_t*), dxmath.xmint3_ctor_3
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
 - XMINT3.XMINT3
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- XMINT3
: 
---

# XMINT3 function


## -description


Initializes a new instance of <code>XMINT3</code> from a three element <code>int32_t</code> array argument.

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/9924ed70-e6f8-4040-aab1-977bc3f197e6">XMINT3</a> from a from a three element
  <code>int32_t</code> array argument.
<div class="alert"><b>Note</b>  This constructor is only available under C++.</div><div> </div>

## -parameters




### -param pArray

Three element <code>int32_t</code> array containing the values used to initialize the three components of a new instance of
        <code>XMINT3</code>.


## -remarks



The following pseudocode demonstrates the operation of this constructor:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMINT3 instance;
	instance.x =  pArray[0];
	instance.y =  pArray[1];
	instance.z =  pArray[2];
    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/9924ed70-e6f8-4040-aab1-977bc3f197e6">XMINT3</a>



<a href="https://msdn.microsoft.com/69eb08b8-a533-40cc-8efb-ccb9106e0e24">XMINT3 Constructors</a>
 

 

