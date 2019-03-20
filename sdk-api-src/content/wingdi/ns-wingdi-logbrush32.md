---
UID: NS:wingdi.tagLOGBRUSH32
title: LOGBRUSH32 (wingdi.h)
author: windows-sdk-content
description: The LOGBRUSH32 structure defines the style, color, and pattern of a physical brush.
old-location: gdi\logbrush32.htm
tech.root: gdi
ms.assetid: 8e2053a9-d7b6-4bf7-b915-4c3871a46b37
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPLOGBRUSH32, *NPLOGBRUSH32, *PLOGBRUSH32, LOGBRUSH32, LOGBRUSH32 structure [Windows GDI], PLOGBRUSH32, PLOGBRUSH32 structure pointer [Windows GDI], _win32_LOGBRUSH32_str, gdi.logbrush32, wingdi/LOGBRUSH32, wingdi/PLOGBRUSH32"
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
 - LOGBRUSH32
product: Windows
targetos: Windows
req.typenames: LOGBRUSH32, *PLOGBRUSH32, *NPLOGBRUSH32, *LPLOGBRUSH32
req.redist: 
---

# LOGBRUSH32 structure


## -description



The <b>LOGBRUSH32</b> structure defines the style, color, and pattern of a physical brush. It is similar to <a href="https://msdn.microsoft.com/ded2c7a4-2248-4d01-95c6-ab4050719094">LOGBRUSH</a>, but it is used to maintain compatibility between 32-bit platforms and 64-bit platforms when we record the metafile record on one platform and then play it on another. Thus, it is only used in <a href="https://msdn.microsoft.com/fd87d52a-1227-48ba-8b7e-a8fd007c9d01">EMRCREATEBRUSHINDIRECT</a>. If the code will only be on one platform, <b>LOGBRUSH</b> is sufficient.




## -struct-fields




### -field lbStyle

The brush style. The <b>lbStyle</b> member must be one of the following styles.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td>BS_DIBPATTERN</td>
<td>A pattern brush defined by a device-independent bitmap (DIB) specification. If <b>lbStyle</b> is BS_DIBPATTERN, the <b>lbHatch</b> member contains a handle to a packed DIB. For more information, see discussion in <b>lbHatch</b>.</td>
</tr>
<tr>
<td>BS_DIBPATTERN8X8</td>
<td>Same as BS_DIBPATTERN.</td>
</tr>
<tr>
<td>BS_DIBPATTERNPT</td>
<td>A pattern brush defined by a device-independent bitmap (DIB) specification. If <b>lbStyle</b> is BS_DIBPATTERNPT, the <b>lbHatch</b> member contains a pointer to a packed DIB. For more information, see discussion in <b>lbHatch</b>.</td>
</tr>
<tr>
<td>BS_HATCHED</td>
<td>Hatched brush.</td>
</tr>
<tr>
<td>BS_HOLLOW</td>
<td>Hollow brush.</td>
</tr>
<tr>
<td>BS_NULL</td>
<td>Same as BS_HOLLOW.</td>
</tr>
<tr>
<td>BS_PATTERN</td>
<td>Pattern brush defined by a memory bitmap.</td>
</tr>
<tr>
<td>BS_PATTERN8X8</td>
<td>Same as BS_PATTERN.</td>
</tr>
<tr>
<td>BS_SOLID</td>
<td>Solid brush.</td>
</tr>
</table>
 


### -field lbColor

The color in which the brush is to be drawn. If <b>lbStyle</b> is the BS_HOLLOW or BS_PATTERN style, <b>lbColor</b> is ignored.

If <b>lbStyle</b> is BS_DIBPATTERN or BS_DIBPATTERNPT, the low-order word of <b>lbColor</b> specifies whether the <b>bmiColors</b> members of the <a href="https://msdn.microsoft.com/84cc51e8-78f3-4ee6-bc08-94feff89afb0">BITMAPINFO</a> structure contain explicit red, green, blue (RGB) values or indexes into the currently realized logical palette. The <b>lbColor</b> member must be one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td>DIB_PAL_COLORS</td>
<td>The color table consists of an array of 16-bit indexes into the currently realized logical palette.</td>
</tr>
<tr>
<td>DIB_RGB_COLORS</td>
<td>The color table contains literal RGB values.</td>
</tr>
</table>
 

If <b>lbStyle</b> is BS_HATCHED or BS_SOLID, <b>lbColor</b> is a <a href="https://msdn.microsoft.com/b87d3de2-7a13-44ef-8253-c6851a75fa54">COLORREF</a> color value. To create a <b>COLORREF</b> color value, use the <a href="https://msdn.microsoft.com/e1dcb5f8-c026-4a4e-8541-928a057bf0ae">RGB</a> macro.


### -field lbHatch

A hatch style. The meaning depends on the brush style defined by <b>lbStyle</b>.

If <b>lbStyle</b> is BS_DIBPATTERN, the <b>lbHatch</b> member contains a handle to a packed DIB. To obtain this handle, an application calls the <a href="https://msdn.microsoft.com/06886545-bd5c-4d81-b1c3-dfa7e146e43a">GlobalAlloc</a> function with GMEM_MOVEABLE (or <a href="https://msdn.microsoft.com/da8cd2be-ff4c-4da5-813c-8759a58228c9">LocalAlloc</a> with LMEM_MOVEABLE) to allocate a block of memory and then fills the memory with the packed DIB. A packed DIB consists of a <a href="https://msdn.microsoft.com/84cc51e8-78f3-4ee6-bc08-94feff89afb0">BITMAPINFO</a> structure immediately followed by the array of bytes that define the pixels of the bitmap.

If <b>lbStyle</b> is BS_DIBPATTERNPT, the <b>lbHatch</b> member contains a pointer to a packed DIB. The pointer derives from the memory block created by <a href="https://msdn.microsoft.com/da8cd2be-ff4c-4da5-813c-8759a58228c9">LocalAlloc</a> with LMEM_FIXED set or by <a href="https://msdn.microsoft.com/06886545-bd5c-4d81-b1c3-dfa7e146e43a">GlobalAlloc</a> with GMEM_FIXED set, or it is the pointer returned by a call like <a href="https://msdn.microsoft.com/a9432e28-9fbd-4a7e-8dce-fad3da04804a">LocalLock</a> (handle_to_the_dib). A packed DIB consists of a <a href="https://msdn.microsoft.com/84cc51e8-78f3-4ee6-bc08-94feff89afb0">BITMAPINFO</a> structure immediately followed by the array of bytes that define the pixels of the bitmap.

If <b>lbStyle</b> is BS_HATCHED, the <b>lbHatch</b> member specifies the orientation of the lines used to create the hatch. It can be one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td>HS_BDIAGONAL</td>
<td>A 45-degree upward, left-to-right hatch</td>
</tr>
<tr>
<td>HS_CROSS</td>
<td>Horizontal and vertical cross-hatch</td>
</tr>
<tr>
<td>HS_DIAGCROSS</td>
<td>45-degree crosshatch</td>
</tr>
<tr>
<td>HS_FDIAGONAL</td>
<td>A 45-degree downward, left-to-right hatch</td>
</tr>
<tr>
<td>HS_HORIZONTAL</td>
<td>Horizontal hatch</td>
</tr>
<tr>
<td>HS_VERTICAL</td>
<td>Vertical hatch</td>
</tr>
</table>
 

If <b>lbStyle</b> is BS_PATTERN, <b>lbHatch</b> is a handle to the bitmap that defines the pattern. The bitmap cannot be a DIB section bitmap, which is created by the <a href="https://msdn.microsoft.com/9276ec84-2860-42be-a9f8-d4efb8d25eec">CreateDIBSection</a> function.

If <b>lbStyle</b> is BS_SOLID or BS_HOLLOW, <b>lbHatch</b> is ignored.


## -remarks



Although <b>lbColor</b> controls the foreground color of a hatch brush, the <a href="https://msdn.microsoft.com/60e4467a-14ab-421e-b174-4b9c0134ce72">SetBkMode</a> and <a href="https://msdn.microsoft.com/9163370b-19c5-4c23-9197-793e4b8d50c4">SetBkColor</a> functions control the background color.

Brushes can be created from bitmaps or DIBs larger than 8 by 8 pixels.




## -see-also




<a href="https://msdn.microsoft.com/84cc51e8-78f3-4ee6-bc08-94feff89afb0">BITMAPINFO</a>



<a href="https://msdn.microsoft.com/30fa46f7-c22e-4b37-ac8c-eece8df28611">Brush Structures</a>



<a href="https://msdn.microsoft.com/b8912842-87d6-4d97-83ce-53d18cbedc74">Brushes Overview</a>



<a href="https://msdn.microsoft.com/b87d3de2-7a13-44ef-8253-c6851a75fa54">COLORREF</a>



<a href="https://msdn.microsoft.com/9276ec84-2860-42be-a9f8-d4efb8d25eec">CreateDIBSection</a>



<a href="https://msdn.microsoft.com/fd87d52a-1227-48ba-8b7e-a8fd007c9d01">EMRCREATEBRUSHINDIRECT</a>



<a href="https://msdn.microsoft.com/ded2c7a4-2248-4d01-95c6-ab4050719094">LOGBRUSH</a>



<a href="https://msdn.microsoft.com/e1dcb5f8-c026-4a4e-8541-928a057bf0ae">RGB</a>



<a href="https://msdn.microsoft.com/9163370b-19c5-4c23-9197-793e4b8d50c4">SetBkColor</a>



<a href="https://msdn.microsoft.com/60e4467a-14ab-421e-b174-4b9c0134ce72">SetBkMode</a>
 

 

