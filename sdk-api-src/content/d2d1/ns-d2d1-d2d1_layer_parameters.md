---
UID: NS:d2d1.D2D1_LAYER_PARAMETERS
title: D2D1_LAYER_PARAMETERS
author: windows-sdk-content
description: Contains the content bounds, mask information, opacity settings, and other options for a layer resource.
old-location: direct2d\D2D1_LAYER_PARAMETERS.htm
tech.root: direct2d
ms.assetid: ce575df6-9464-4672-9a0e-ff7e016d9354
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D2D1_LAYER_PARAMETERS, D2D1_LAYER_PARAMETERS structure [Direct2D], d2d1/D2D1_LAYER_PARAMETERS, direct2d.D2D1_LAYER_PARAMETERS
ms.topic: struct
req.header: d2d1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
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
 - d2d1.h
api_name:
 - D2D1_LAYER_PARAMETERS
product: Windows
targetos: Windows
req.typenames: D2D1_LAYER_PARAMETERS
req.redist: 
---

# D2D1_LAYER_PARAMETERS structure


## -description


Contains the content bounds, mask information, opacity settings, and other options for a layer resource. 


## -struct-fields




### -field contentBounds

Type: <b><a href="https://msdn.microsoft.com/a961c0e3-fb76-4c07-b76e-47d8c09ada08">D2D1_RECT_F</a></b>

The content bounds of the layer. Content outside these bounds is not guaranteed to render.


### -field geometricMask

Type: <b><a href="https://msdn.microsoft.com/be4ab801-64f6-48f9-8f62-d0492cc438b1">ID2D1Geometry</a>*</b>

The geometric mask specifies the area of the layer that is composited into the render target. 


### -field maskAntialiasMode

Type: <b><a href="https://msdn.microsoft.com/3ca12155-6dd0-41bb-8778-3387422c4ffe">D2D1_ANTIALIAS_MODE</a></b>

A value that specifies the antialiasing mode for the geometricMask.  


### -field maskTransform

Type: <b><a href="https://msdn.microsoft.com/f05d7555-6482-4eea-950f-7b443892cc1f">D2D1_MATRIX_3X2_F</a></b>

A value that specifies the transform that is applied to the geometric mask when composing the layer.


### -field opacity

Type: <b>FLOAT</b>

An opacity value that is applied uniformly to all resources in the layer when compositing to the target.


### -field opacityBrush

Type: <b><a href="https://msdn.microsoft.com/5b8f6ff8-ba52-4d30-9bea-3de89793c868">ID2D1Brush</a>*</b>

A brush that is used to modify the opacity of the layer. The brush 
is mapped to the layer, and the alpha channel of each mapped brush pixel is multiplied against the corresponding layer pixel. 


### -field layerOptions

Type: <b><a href="https://msdn.microsoft.com/d278211a-e99c-429d-9752-45c305f52ed8">D2D1_LAYER_OPTIONS</a></b>

A value that specifies whether the layer intends to render text with ClearType antialiasing.


## -see-also




<a href="https://msdn.microsoft.com/22d161fb-8470-49cc-a523-309f90643ea9">Layers Overview</a>
 

 

