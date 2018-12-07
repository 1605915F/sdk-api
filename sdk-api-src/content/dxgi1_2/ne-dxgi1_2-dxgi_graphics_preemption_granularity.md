---
UID: NE:dxgi1_2.DXGI_GRAPHICS_PREEMPTION_GRANULARITY
title: DXGI_GRAPHICS_PREEMPTION_GRANULARITY
author: windows-sdk-content
description: Identifies the granularity at which the graphics processing unit (GPU) can be preempted from performing its current graphics rendering task.
old-location: direct3ddxgi\dxgi_graphics_preemption_granularity.htm
tech.root: direct3ddxgi
ms.assetid: B1372869-EFDE-49DD-BCF8-D4F59AFE8E7E
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DXGI_GRAPHICS_PREEMPTION_DMA_BUFFER_BOUNDARY, DXGI_GRAPHICS_PREEMPTION_GRANULARITY, DXGI_GRAPHICS_PREEMPTION_GRANULARITY enumeration [DXGI], DXGI_GRAPHICS_PREEMPTION_INSTRUCTION_BOUNDARY, DXGI_GRAPHICS_PREEMPTION_PIXEL_BOUNDARY, DXGI_GRAPHICS_PREEMPTION_PRIMITIVE_BOUNDARY, DXGI_GRAPHICS_PREEMPTION_TRIANGLE_BOUNDARY, direct3ddxgi.dxgi_graphics_preemption_granularity, dxgi1_2/DXGI_GRAPHICS_PREEMPTION_DMA_BUFFER_BOUNDARY, dxgi1_2/DXGI_GRAPHICS_PREEMPTION_GRANULARITY, dxgi1_2/DXGI_GRAPHICS_PREEMPTION_INSTRUCTION_BOUNDARY, dxgi1_2/DXGI_GRAPHICS_PREEMPTION_PIXEL_BOUNDARY, dxgi1_2/DXGI_GRAPHICS_PREEMPTION_PRIMITIVE_BOUNDARY, dxgi1_2/DXGI_GRAPHICS_PREEMPTION_TRIANGLE_BOUNDARY
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: dxgi1_2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
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
 - DXGI1_2.h
api_name:
 - DXGI_GRAPHICS_PREEMPTION_GRANULARITY
product: Windows
targetos: Windows
req.typenames: DXGI_GRAPHICS_PREEMPTION_GRANULARITY
req.redist: 
---

# DXGI_GRAPHICS_PREEMPTION_GRANULARITY enumeration


## -description


Identifies the granularity at which the graphics processing unit (GPU) can be preempted from performing its current graphics rendering task.


## -enum-fields




### -field DXGI_GRAPHICS_PREEMPTION_DMA_BUFFER_BOUNDARY

Indicates the preemption granularity as a DMA buffer.


### -field DXGI_GRAPHICS_PREEMPTION_PRIMITIVE_BOUNDARY

Indicates the preemption granularity as a graphics primitive. A primitive is a section in a DMA buffer and can be a group of triangles.


### -field DXGI_GRAPHICS_PREEMPTION_TRIANGLE_BOUNDARY

Indicates the preemption granularity as a triangle. A triangle is a part of a primitive.


### -field DXGI_GRAPHICS_PREEMPTION_PIXEL_BOUNDARY

Indicates the preemption granularity as a pixel. A pixel is a part of a triangle.


### -field DXGI_GRAPHICS_PREEMPTION_INSTRUCTION_BOUNDARY

Indicates the preemption granularity as a graphics instruction. A graphics instruction operates on a pixel.


## -remarks



You call the <a href="https://msdn.microsoft.com/DC1A054D-4092-4865-A6EF-B936891AA470">IDXGIAdapter2::GetDesc2</a> method to retrieve the granularity level at which the GPU can be preempted from performing its current graphics rendering task. The operating system specifies the graphics granularity level in the  <b>GraphicsPreemptionGranularity</b> member of the <a href="https://msdn.microsoft.com/AE34913A-84D8-49DB-A736-15AECA9989F9">DXGI_ADAPTER_DESC2</a> structure.

The following figure shows granularity of graphics rendering tasks.

<img alt="Graphics Rendering Granularity" src="./images/Graphics_Preempt.png"/>



## -see-also




<a href="https://msdn.microsoft.com/c4574c89-dee2-4841-9318-5383cf417111">DXGI Enumerations</a>



<a href="https://msdn.microsoft.com/AE34913A-84D8-49DB-A736-15AECA9989F9">DXGI_ADAPTER_DESC2</a>
 

 

