---
UID: NF:amvideo.COLORS
title: COLORS macro (amvideo.h)
author: windows-sdk-content
description: The COLORS macro retrieves the palette entries from a VIDEOINFO structure.
old-location: dshow\colors.htm
tech.root: DirectShow
ms.assetid: 32541ee4-53ef-4f0a-b823-bb475a93a195
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: COLORS, COLORS function [DirectShow], amvideo/COLORS, dshow.colors
ms.topic: macro
req.header: amvideo.h
req.include-header: Streams.h
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
req.lib: Strmbase.lib (retail builds); Strmbasd.lib (debug builds)
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Strmbase.lib
 - Strmbase.dll
 - Strmbasd.lib
 - Strmbasd.dll
api_name:
 - COLORS
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# COLORS macro


## -description


The COLORS macro retrieves the palette entries from a <a href="https://msdn.microsoft.com/en-us/library/Dd407323(v=VS.85).aspx">VIDEOINFO</a> structure. 


## -parameters




### -param pbmi

Pointer to a <a href="https://msdn.microsoft.com/en-us/library/Dd407323(v=VS.85).aspx">VIDEOINFO</a> structure. 


## -remarks



This macro calculates the address as an offset from the start of the <a href="https://msdn.microsoft.com/153c08a8-d32c-4e9d-9da9-b915eb172327">BITMAPINFOHEADER</a> structure, using the value of <b>bmiHeader.biSize</b>. Make sure to initialize the <a href="https://msdn.microsoft.com/en-us/library/Dd407323(v=VS.85).aspx">VIDEOINFO</a> structure before calling this macro.




## -see-also




<a href="https://msdn.microsoft.com/02401edc-362b-4f6c-b10b-c46b30b3ebe7">Video and Image Functions</a>
 

 

