---
UID: NF:mileffects.IMILBitmapEffectPrimitive.TransformRect
title: IMILBitmapEffectPrimitive::TransformRect
author: windows-sdk-content
description: Transforms the output of the given rectangle.
old-location: wibe\_wibe_imilbitmapeffectprimitive_transformrect.htm
tech.root: wibe
ms.assetid: VS|wibe|~\wibelh\reference\ifaces\imilbitmapeffectprimitive\transformrect.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMILBitmapEffectPrimitive interface [WPF Bitmap Effects],TransformRect method, IMILBitmapEffectPrimitive.TransformRect, IMILBitmapEffectPrimitive::TransformRect, TransformRect, TransformRect method [WPF Bitmap Effects], TransformRect method [WPF Bitmap Effects],IMILBitmapEffectPrimitive interface, _wibe_imilbitmapeffectprimitive_transformrect, mileffects/IMILBitmapEffectPrimitive::TransformRect, wibe._wibe_imilbitmapeffectprimitive_transformrect
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mileffects.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mileffects.idl
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
 - COM
api_location:
 - Mileffects.h
api_name:
 - IMILBitmapEffectPrimitive.TransformRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: Microsoft .Net 3.0
---

# IMILBitmapEffectPrimitive::TransformRect


## -description


Transforms the output of the given rectangle.


## -parameters




### -param uiIndex [in]

Type: <b>ULONG</b>

A zero based index value indicating the output pin through which to transform the rectangle.


### -param p [in, out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms735228(v=VS.85).aspx">MIL_RECTD</a>*</b>

A pointer to the rectangle to transform.


### -param fForwardTransform [in]

Type: <b>VARIANT_BOOL</b>

A value indicating whether the rectangle is being transformed from front to back in the effects graph.


### -param pContext [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms735245(v=VS.85).aspx">IMILBitmapEffectRenderContext</a>*</b>

The render context to use for the transformation.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.



