---
UID: NF:d2d1_1.ID2D1DeviceContext.DrawImage(ID2D1Effect,D2D1_INTERPOLATION_MODE,D2D1_COMPOSITE_MODE)
title: ID2D1DeviceContext::DrawImage(ID2D1Effect,D2D1_INTERPOLATION_MODE,D2D1_COMPOSITE_MODE) (d2d1_1.h)
author: windows-sdk-content
description: Draws an image to the device context.
old-location: direct2d\id2d1devicecontext_drawimage4.htm
tech.root: Direct2D
ms.assetid: D2524021-3775-413F-9AC8-D5175B36AABB
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DrawImage, DrawImage method [Direct2D], DrawImage method [Direct2D],ID2D1DeviceContext interface, ID2D1DeviceContext interface [Direct2D],DrawImage method, ID2D1DeviceContext.DrawImage, ID2D1DeviceContext.DrawImage(ID2D1Effect,D2D1_INTERPOLATION_MODE,D2D1_COMPOSITE_MODE), ID2D1DeviceContext::DrawImage, ID2D1DeviceContext::DrawImage(ID2D1Effect,D2D1_INTERPOLATION_MODE,D2D1_COMPOSITE_MODE), d2d1_1/ID2D1DeviceContext::DrawImage, direct2d.id2d1devicecontext_drawimage4
ms.topic: method
req.header: d2d1_1.h
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
req.dll: D2d1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D2d1.dll
api_name:
 - ID2D1DeviceContext.DrawImage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1DeviceContext::DrawImage(ID2D1Effect,D2D1_INTERPOLATION_MODE,D2D1_COMPOSITE_MODE)


## -description


Draws an image to the device context.


## -parameters




### -param effect [in]

Type: <b><a href="https://msdn.microsoft.com/e90d1830-c356-48f1-ac7b-1d94c8c26569">ID2D1Effect</a>*</b>

The effect to be drawn to the device context.


### -param interpolationMode

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh447004(v=VS.85).aspx">D2D1_INTERPOLATION_MODE</a></b>

The interpolation mode that will be used to scale the image if necessary.


### -param compositeMode

Type: <b><a href="https://msdn.microsoft.com/4f01e805-aed7-4bfc-9793-42a9fdde3473">D2D1_COMPOSITE_MODE</a></b>

The composite mode that will be applied to the limits of the currently selected clip. The default value is <b>D2D1_COMPOSITE_MODE_SOURCE_OVER</b>


## -returns



This method does not return a value.




## -remarks



If <i>interpolationMode</i> is <b>D2D1_INTERPOLATION_MODE_HIGH_QUALITY</b>, different scalers will be used depending on the scale factor implied by the world transform.

Any invalid rectangles accumulated on any effect that is drawn by this call will be discarded regardless of which portion of the image rectangle is drawn.

If <i>compositeMode</i> is <b>D2D1_COMPOSITE_MODE_SOURCE_OVER</b>, <a href="https://msdn.microsoft.com/c41d8a79-280a-451e-b07b-f904d07da5c7">DrawImage</a> will use the currently selected primitive blend specified by <a href="https://msdn.microsoft.com/be04c9f7-397f-468e-91c0-3b11c68b489f">ID2D1DeviceContext::SetPrimitiveBlend</a>. If <i>compositeMode</i> is not <b>D2D1_COMPOSITE_MODE_SOURCE_OVER</b>, the image will be extended to transparent up to the current axis-aligned clip.

If there is an image rectangle and a world transform, this is equivalent to inserting a clip effect to represent the image rectangle and a 2D affine transform to take into account the world transform.




## -see-also




<a href="https://msdn.microsoft.com/e58216ea-e6b5-450f-a0ea-b879aa5dff38">ID2D1Bitmap</a>



<a href="https://msdn.microsoft.com/669a9377-248c-4a86-b447-ed117fff43a6">ID2D1Bitmap1</a>



<a href="https://msdn.microsoft.com/a54dd628-c2a2-4b04-9ced-7749a395f187">ID2D1DeviceContext</a>



<a href="https://msdn.microsoft.com/e90d1830-c356-48f1-ac7b-1d94c8c26569">ID2D1Effect</a>



<a href="https://msdn.microsoft.com/9f7b4546-edbe-4000-a4ce-1a69563ebf9d">ID2D1Image</a>
 

 

