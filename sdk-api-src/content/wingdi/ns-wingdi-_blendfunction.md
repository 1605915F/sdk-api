---
UID: NS:wingdi._BLENDFUNCTION
title: "_BLENDFUNCTION"
author: windows-sdk-content
description: The BLENDFUNCTION structure controls blending by specifying the blending functions for source and destination bitmaps.
old-location: gdi\blendfunction.htm
tech.root: gdi
ms.assetid: d1371d72-c408-4484-845e-d4ea2bc3115d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PBLENDFUNCTION, BLENDFUNCTION, BLENDFUNCTION structure [Windows GDI], LPBLENDFUNCTION, LPBLENDFUNCTION structure pointer [Windows GDI], PBLENDFUNCTION, PBLENDFUNCTION structure pointer [Windows GDI], _BLENDFUNCTION, _win32_BLENDFUNCTION_str, gdi.blendfunction, wingdi/BLENDFUNCTION, wingdi/LPBLENDFUNCTION, wingdi/PBLENDFUNCTION"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: wingdi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Wingdi.h
api_name:
 - BLENDFUNCTION
product: Windows
targetos: Windows
req.typenames: BLENDFUNCTION, *PBLENDFUNCTION
req.redist: 
---

# _BLENDFUNCTION structure


## -description



The <b>BLENDFUNCTION</b> structure controls blending by specifying the blending functions for source and destination bitmaps.




## -struct-fields




### -field BlendOp

The source blend operation. Currently, the only source and destination blend operation that has been defined is AC_SRC_OVER. For details, see the following Remarks section.


### -field BlendFlags

Must be zero.


### -field SourceConstantAlpha

Specifies an alpha transparency value to be used on the entire source bitmap. The <b>SourceConstantAlpha</b> value is combined with any per-pixel alpha values in the source bitmap. If you set <b>SourceConstantAlpha</b> to 0, it is assumed that your image is transparent. Set the <b>SourceConstantAlpha</b> value to 255 (opaque) when you only want to use per-pixel alpha values.


### -field AlphaFormat

This member controls the way the source and destination bitmaps are interpreted. <b>AlphaFormat</b> has the following value.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td>AC_SRC_ALPHA</td>
<td>This flag is set when the bitmap has an Alpha channel (that is, per-pixel alpha). Note that the APIs use premultiplied alpha, which means that the red, green and blue channel values in the bitmap must be premultiplied with the alpha channel value. For example, if the alpha channel value is x, the red, green and blue channels must be multiplied by x and divided by 0xff prior to the call.</td>
</tr>
</table>
 


## -remarks



When the <b>AlphaFormat</b> member is AC_SRC_ALPHA, the source bitmap must be 32 bpp. If it is not, the <a href="https://msdn.microsoft.com/4624aa31-7e19-4506-ac70-9b3c98a8215d">AlphaBlend</a> function will fail.

When the <b>BlendOp</b> member is AC_SRC_OVER, the source bitmap is placed over the destination bitmap based on the alpha values of the source pixels.

If the source bitmap has no per-pixel alpha value (that is, AC_SRC_ALPHA is not set), the <b>SourceConstantAlpha</b> value determines the blend of the source and destination bitmaps, as shown in the following table. Note that SCA is used for <b>SourceConstantAlpha</b> here. Also, SCA is divided by 255 because it has a value that ranges from 0 to 255.

<table>
<tr>
<td>Dst.Red</td>
<td>= Src.Red * (SCA/255.0)</td>
<td>+ Dst.Red * (1.0 - (SCA/255.0))</td>
</tr>
<tr>
<td>Dst.Green</td>
<td>= Src.Green * (SCA/255.0)</td>
<td>+ Dst.Green * (1.0 - (SCA/255.0))</td>
</tr>
<tr>
<td>Dst.Blue</td>
<td>= Src.Blue * (SCA/255.0)</td>
<td>+ Dst.Blue * (1.0 - (SCA/255.0))</td>
</tr>
</table>
 

If the destination bitmap has an alpha channel, then the blend is as follows.

<table>
<tr>
<td>Dst.Alpha</td>
<td>= Src.Alpha * (SCA/255.0)</td>
<td>+ Dst.Alpha * (1.0 - (SCA/255.0))</td>
</tr>
</table>
 

If the source bitmap does not use <b>SourceConstantAlpha</b> (that is, it equals 0xFF), the per-pixel alpha determines the blend of the source and destination bitmaps, as shown in the following table.

<table>
<tr>
<td>Dst.Red</td>
<td>= Src.Red</td>
<td>+ (1 - Src.Alpha) * Dst.Red</td>
</tr>
<tr>
<td>Dst.Green</td>
<td>= Src.Green</td>
<td>+ (1 - Src.Alpha) * Dst.Green</td>
</tr>
<tr>
<td>Dst.Blue</td>
<td>= Src.Blue</td>
<td>+ (1 - Src.Alpha) * Dst.Blue</td>
</tr>
</table>
 

If the destination bitmap has an alpha channel, then the blend is as follows.

<table>
<tr>
<td>Dest.alpha</td>
<td>= Src.Alpha</td>
<td>+ (1 - SrcAlpha) * Dst.Alpha</td>
</tr>
</table>
 

If the source has both the <b>SourceConstantAlpha</b> (that is, it is not 0xFF) and per-pixel alpha, the source is pre-multiplied by the <b>SourceConstantAlpha</b> and then the blend is based on the per-pixel alpha. The following tables show this. Note that <b>SourceConstantAlpha</b> is divided by 255 because it has a value that ranges from 0 to 255.

<table>
<tr>
<td>Src.Red</td>
<td>= Src.Red</td>
<td>* SourceConstantAlpha / 255.0;</td>
</tr>
<tr>
<td>Src.Green</td>
<td>= Src.Green</td>
<td>* SourceConstantAlpha / 255.0;</td>
</tr>
<tr>
<td>Src.Blue</td>
<td>= Src.Blue</td>
<td>* SourceConstantAlpha / 255.0;</td>
</tr>
<tr>
<td>Src.Alpha</td>
<td>= Src.Alpha</td>
<td>* SourceConstantAlpha / 255.0;</td>
</tr>
<tr>
<td>Dst.Red</td>
<td>= Src.Red</td>
<td>+ (1 - Src.Alpha) * Dst.Red</td>
</tr>
<tr>
<td>Dst.Green</td>
<td>= Src.Green</td>
<td>+ (1 - Src.Alpha) * Dst.Green</td>
</tr>
<tr>
<td>Dst.Blue</td>
<td>= Src.Blue</td>
<td>+ (1 - Src.Alpha) * Dst.Blue</td>
</tr>
<tr>
<td>Dst.Alpha</td>
<td>= Src.Alpha</td>
<td>+ (1 - Src.Alpha) * Dst.Alpha</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/4624aa31-7e19-4506-ac70-9b3c98a8215d">AlphaBlend</a>



<a href="https://msdn.microsoft.com/29f8237f-9c7e-41a7-90b1-5f048fcc74a6">Bitmap Structures</a>



<a href="https://msdn.microsoft.com/ff0a5ae3-ae2e-4417-b5e5-0f9871c03964">Bitmaps Overview</a>
 

 

