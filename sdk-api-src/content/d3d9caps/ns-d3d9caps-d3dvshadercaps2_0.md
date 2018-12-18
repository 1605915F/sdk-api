---
UID: NS:d3d9caps._D3DVSHADERCAPS2_0
title: D3DVSHADERCAPS2_0
author: windows-sdk-content
description: Vertex shader caps.
old-location: direct3d9\d3dvshadercaps2_0.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\d3dvshadercaps2_0.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 85a71d10-ae0f-bdc3-e929-6d1ff3c0b356, D3DVSHADERCAPS2_0, D3DVSHADERCAPS2_0 structure [Direct3D 9], LPD3DVSHADERCAPS2_0, LPD3DVSHADERCAPS2_0 structure pointer [Direct3D 9], d3d9caps/D3DVSHADERCAPS2_0, d3d9caps/LPD3DVSHADERCAPS2_0, direct3d9.d3dvshadercaps2_0
ms.topic: struct
req.header: d3d9caps.h
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
 - D3D9Caps.h
api_name:
 - D3DVSHADERCAPS2_0
product: Windows
targetos: Windows
req.typenames: D3DVSHADERCAPS2_0
req.redist: 
---

# D3DVSHADERCAPS2_0 structure


## -description


Vertex shader caps.


## -struct-fields




### -field Caps

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a></b>

Instruction predication is supported if this value is nonzero. See <a href="https://msdn.microsoft.com/bfead3f8-f7fe-4fc1-939f-8e5fbc3e0adf">setp_comp - vs</a>.


### -field DynamicFlowControlDepth

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">INT</a></b>

 Either 0 or 24, which represents the depth of the dynamic flow control instruction nesting. See <a href="https://msdn.microsoft.com/c1321957-4ba5-45d0-984a-4f4267221c59">D3DVS20CAPS</a>.


### -field NumTemps

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">INT</a></b>

The number of temporary registers supported. See <a href="https://msdn.microsoft.com/c1321957-4ba5-45d0-984a-4f4267221c59">D3DVS20CAPS</a>.


### -field StaticFlowControlDepth

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">INT</a></b>

The depth of nesting of the <a href="https://msdn.microsoft.com/1d587559-ef4b-40a5-bce5-49354d11ff91">loop - vs</a>/<a href="https://msdn.microsoft.com/0f795557-b5b0-45e6-8134-9558619f80fc">rep - vs</a> and <a href="https://msdn.microsoft.com/3c1ec529-1ee4-40d9-8ce5-f8e7a61fde9c">call - vs</a>/<a href="https://msdn.microsoft.com/9be030b9-fa21-459f-bd6c-f34ad6f177fc">callnz bool - vs</a> instructions. See <a href="https://msdn.microsoft.com/c1321957-4ba5-45d0-984a-4f4267221c59">D3DVS20CAPS</a>.


## -see-also




<a href="https://msdn.microsoft.com/44457b7b-a1f7-4019-b971-8ec2334d3313">D3DCAPS9</a>



<a href="https://msdn.microsoft.com/924b05cb-9af0-4774-8fe3-74b2484505a4">D3DPSHADERCAPS2_0</a>



<a href="https://msdn.microsoft.com/0a13cb04-10cb-48a6-a709-ad4a56459f02">Direct3D Structures</a>
 

 

