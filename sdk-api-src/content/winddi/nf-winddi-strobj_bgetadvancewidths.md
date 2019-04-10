---
UID: NF:winddi.STROBJ_bGetAdvanceWidths
title: STROBJ_bGetAdvanceWidths function (winddi.h)
author: windows-sdk-content
description: The STROBJ_bGetAdvanceWidths function retrieves an array of vectors specifying the probable widths of glyphs making up a specified string.
old-location: display\strobj_bgetadvancewidths.htm
tech.root: display
ms.assetid: 298d75a7-2e9b-47df-98ba-d159429a6301
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: STROBJ_bGetAdvanceWidths, STROBJ_bGetAdvanceWidths function [Display Devices], display.strobj_bgetadvancewidths, gdifncs_d101c29f-374a-4e66-801c-beba0805f070.xml, winddi/STROBJ_bGetAdvanceWidths
ms.topic: function
req.header: winddi.h
req.include-header: Winddi.h
req.target-type: Universal
req.target-min-winverclnt: Available in Windows 2000 and later versions of the Windows operating systems.
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
req.lib: Win32k.lib
req.dll: Win32k.sys
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Win32k.sys
api_name:
 - STROBJ_bGetAdvanceWidths
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# STROBJ_bGetAdvanceWidths function


## -description


The <b>STROBJ_bGetAdvanceWidths</b> function retrieves an array of vectors specifying the probable widths of glyphs making up a specified string.


## -parameters




### -param pso

Is a caller-supplied pointer to a <a href="https://msdn.microsoft.com/efe53cb8-39b9-4931-bac2-9c61efd9d457">STROBJ</a> structure describing a text string. This is typically the STROBJ structure received by the driver's <a href="https://msdn.microsoft.com/f2f61687-d833-4d09-8cd5-99e81436c1c1">DrvTextOut</a> function.


### -param iFirst [in]

Is a caller-supplied, zero-based index into the text string supplied by the STROBJ structure. This index represents the first character of the string for which a width is to be returned.


### -param c

Is a caller-supplied count of the number of contiguous characters, starting and the character specified by <i>iFirst</i>, for which width values are to be returned.


### -param pptqD

Is a caller-supplied pointer to a <i>c</i>-sized array of POINTQF structures to receive character widths in (28.36, 28.36) format. For a description of this data type, see <a href="https://msdn.microsoft.com/2054aa16-6d86-4db3-8b16-4570b0374e23">GDI Data Types</a>.


## -returns



If the operation succeeds, the function returns <b>TRUE</b>; otherwise it returns <b>FALSE</b>.




## -remarks



The <b>STROBJ_bGetAdvanceWidths</b> function is useful to printer drivers that call <a href="https://msdn.microsoft.com/d5ffe766-843d-4e42-8cc8-bc405e78a2fd">STROBJ_bEnumPositionsOnly</a> instead of <a href="https://msdn.microsoft.com/82cb12ff-2baa-4291-849c-dab9d01fa39b">STROBJ_bEnum</a>. The function fills in the <i>pptqD</i> array with the probable widths of a string's glyphs, and can be used to calculate the printer position after a string as been rendered by the printer, if the printer's glyph rendering hardware does not return exact character widths.

Note that glyph positions returned by <b>STROBJ_bEnumPositionsOnly</b> do not necessarily correspond exactly to the widths returned by <b>STROBJ_bGetAdvanceWidths.</b>




## -see-also




<a href="https://msdn.microsoft.com/f2f61687-d833-4d09-8cd5-99e81436c1c1">DrvTextOut</a>



<a href="https://msdn.microsoft.com/efe53cb8-39b9-4931-bac2-9c61efd9d457">STROBJ</a>



<a href="https://msdn.microsoft.com/82cb12ff-2baa-4291-849c-dab9d01fa39b">STROBJ_bEnum</a>



<a href="https://msdn.microsoft.com/d5ffe766-843d-4e42-8cc8-bc405e78a2fd">STROBJ_bEnumPositionsOnly</a>
 

 

