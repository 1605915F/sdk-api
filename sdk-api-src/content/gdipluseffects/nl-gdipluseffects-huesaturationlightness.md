---
UID: NL:gdipluseffects.HueSaturationLightness
title: HueSaturationLightness (gdipluseffects.h)
author: windows-sdk-content
description: The HueSaturationLightness class enables you to change the hue, saturation, and lightness of a bitmap.
old-location: gdiplus\_gdiplus_CLASS_HueSaturationLightness_Class.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\huesaturationlightness.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: HueSaturationLightness, HueSaturationLightness class [GDI+], HueSaturationLightness class [GDI+],described, _gdiplus_CLASS_HueSaturationLightness_Class, gdiplus._gdiplus_CLASS_HueSaturationLightness_Class, gdipluseffects/HueSaturationLightness
ms.topic: class
req.header: gdipluseffects.h
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
 - COM
api_location:
 - gdipluseffects.h
api_name:
 - HueSaturationLightness
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# HueSaturationLightness class


## -description


The <b>HueSaturationLightness</b> class enables you to change the hue, saturation, and lightness of a bitmap. Pass the address of a <b>HueSaturationLightness</b> object to the <a href="https://msdn.microsoft.com/en-us/library/ms536058(v=VS.85).aspx">Graphics::DrawImage</a> method or to the <a href="https://msdn.microsoft.com/en-us/library/ms536284(v=VS.85).aspx">Bitmap::ApplyEffect</a> method. To specify the magnitudes of the changes in hue, saturation, and lightness, pass a <a href="https://msdn.microsoft.com/en-us/library/ms534069(v=VS.85).aspx">HueSaturationLightnessParams</a> structure to the <a href="https://msdn.microsoft.com/en-us/library/ms535442(v=VS.85).aspx">HueSaturationLightness::SetParameters</a> method of a <b>HueSaturationLightness</b> object.

