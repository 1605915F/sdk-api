---
UID: NS:winddi._FD_GLYPHSET
title: FD_GLYPHSET (winddi.h)
author: windows-sdk-content
description: The FD_GLYPHSET structure is used to define the mappings from Unicode characters to glyph handles.
old-location: display\fd_glyphset.htm
tech.root: display
ms.assetid: af56f2a0-92a6-4217-8121-944a0b4f26f6
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: "*PFD_GLYPHSET, FD_GLYPHSET, FD_GLYPHSET structure [Display Devices], PFD_GLYPHSET, PFD_GLYPHSET structure pointer [Display Devices], display.fd_glyphset, grstrcts_69cd5b01-58bb-4141-8f1d-26a6258423ce.xml, winddi/FD_GLYPHSET, winddi/PFD_GLYPHSET"
ms.topic: struct
req.header: winddi.h
req.include-header: Winddi.h
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
 - winddi.h
api_name:
 - FD_GLYPHSET
product: Windows
targetos: Windows
req.typenames: FD_GLYPHSET, *PFD_GLYPHSET
req.redist: 
---

# FD_GLYPHSET structure


## -description


The FD_GLYPHSET structure is used to define the mappings from Unicode characters to glyph handles.


## -struct-fields




### -field cjThis

Specifies the size, in bytes, of the structure, including the array of <a href="https://msdn.microsoft.com/01a90280-a7cc-4726-b0a2-68121bdb4686">WCRUN</a> structures.


### -field flAccel

Specifies accelerator flags. This member must be the following value:

<table>
<tr>
<th>Flags</th>
<th>Meaning</th>
</tr>
<tr>
<td>
GS_8BIT_HANDLES

</td>
<td>
All handles are 8-bit quantities.

</td>
</tr>
<tr>
<td>
GS_16BIT_HANDLES

</td>
<td>
All handles are 16-bit quantities. 

</td>
</tr>
<tr>
<td>
GS_UNICODE_HANDLES

</td>
<td>
For all runs in this structure, the handle is obtained by zero extending the Unicode code point.

</td>
</tr>
</table>
 


### -field cGlyphsSupported

Specifies the total number of glyphs in all runs.


### -field cRuns

Specifies the number of <a href="https://msdn.microsoft.com/01a90280-a7cc-4726-b0a2-68121bdb4686">WCRUN</a> structures in the <b>awcrun</b> array.


### -field awcrun

Is an array of <a href="https://msdn.microsoft.com/01a90280-a7cc-4726-b0a2-68121bdb4686">WCRUN</a> structures.


## -see-also




<a href="https://msdn.microsoft.com/29601ea6-9b68-4cdc-a7a1-b6a922524760">DrvQueryFontTree</a>



<a href="https://msdn.microsoft.com/01a90280-a7cc-4726-b0a2-68121bdb4686">WCRUN</a>
 

 

