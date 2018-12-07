---
UID: NF:directxmath.XMVectorATan2Est
title: XMVectorATan2Est function
author: windows-sdk-content
description: Estimates the arctangent of Y/X.
old-location: dxmath\xmvectoratan2est.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.transcendental.XMVectorATan2Est(XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorATan2Est, XMVectorATan2Est, XMVectorATan2Est method [DirectX Math Support APIs], dxmath.xmvectoratan2est
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - XMVectorATan2Est
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorATan2Est function


## -description


Estimates the arctangent of <i>Y</i>/<i>X</i>.


## -parameters




### -param Y [in]

First vector.


### -param X [in]

Second vector.


## -returns



Returns a vector. Each component is an estimate of the arctangent of the corresponding <i>Y</i> component divided by the corresponding <i>X</i> component. 
        Each component is in the range (-PI/2, PI/2).

<code>XMVectorATan2Est</code> returns the following values for the specified special input values.

<table>
<tr>
<th>Input Value</th>
<th>Return Value</th>
</tr>
<tr>
<td>Y == 0 and X &lt; 0</td>
<td>Pi with the same sign as Y</td>
</tr>
<tr>
<td>Y == 0 and X &gt; 0</td>
<td>0 with the same sign as Y</td>
</tr>
<tr>
<td>Y != 0 and X == 0</td>
<td>Pi / 2 with the same sign as Y</td>
</tr>
<tr>
<td>X == -Infinity and Y is finite</td>
<td>Pi with the same sign as Y</td>
</tr>
<tr>
<td>X == +Infinity and Y is finite</td>
<td>0 with the same sign as Y</td>
</tr>
<tr>
<td>Y == Infinity and X is finite</td>
<td>Pi / 2 with the same sign as Y</td>
</tr>
<tr>
<td>Y == Infinity and X == -Infinity</td>
<td>3Pi / 4 with the same sign as Y</td>
</tr>
<tr>
<td>Y == Infinity and X == +Infinity</td>
<td>Pi / 4 with the same sign as Y</td>
</tr>
</table>
 




## -remarks



<code>Est</code> functions offer increased performance at the expense of reduced accuracy.
    <code>Est</code> functions are appropriate for non-critical calculations where accuracy can be sacrificed for speed.
    The exact amount of lost accuracy and speed increase are platform dependent.

This function uses a 9-degree minimax approximation.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/aae12d4a-7758-83df-5376-99d5d94a28c4">Transcendental Vector Functions</a>



<a href="https://msdn.microsoft.com/b7fe0cd6-a447-4123-8715-8f540fdcced6">XMVectorATan</a>



<a href="https://msdn.microsoft.com/f39d7f8e-49a8-428e-b115-e91a9412d13c">XMVectorATan2</a>



<a href="https://msdn.microsoft.com/4b3432aa-535a-4b5a-b878-c26b6d77cfe4">XMVectorATanEst</a>



<a href="https://msdn.microsoft.com/6555d1a8-fb83-4e29-877f-3efb845eb620">XMVectorTan</a>
 

 

