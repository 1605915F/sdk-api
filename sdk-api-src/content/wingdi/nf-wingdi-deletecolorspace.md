---
UID: NF:wingdi.DeleteColorSpace
title: DeleteColorSpace function (wingdi.h)
author: windows-sdk-content
description: The DeleteColorSpace function removes and destroys a specified color space.
old-location: wcs\deletecolorspace.htm
tech.root: WCS
ms.assetid: 5b241224-2994-4533-9629-d2a4b129ce86
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: DeleteColorSpace, DeleteColorSpace function [Windows Color System], _color_DeleteColorSpace, wcs.deletecolorspace, wingdi/DeleteColorSpace
ms.topic: function
req.header: wingdi.h
req.include-header: 
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
req.lib: Gdi32.lib
req.dll: Gdi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - gdi32.dll
 - API-MS-Win-GDI-Internal-Uap-L1-1-0.dll
 - Ext-MS-Win-GDI-Internal-Desktop-L1-1-0.dll
 - GDI32Full.dll
 - GDI32Min.dll
api_name:
 - DeleteColorSpace
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# DeleteColorSpace function


## -description


The <b>DeleteColorSpace</b> function removes and destroys a specified <a href="https://msdn.microsoft.com/en-us/library/Dd371818(v=VS.85).aspx">color space</a>.


## -parameters




### -param hcs

Specifies the handle to a color space to delete.


## -returns



If this function succeeds, the return value is <b>TRUE</b>.

If this function fails, the return value is <b>FALSE</b>.




## -see-also




<a href="https://msdn.microsoft.com/a0623917-0b63-4546-a71a-1e9efa9fe8e5">Basic Color Management Concepts</a>



<a href="https://msdn.microsoft.com/ee9e9502-5514-4070-95fa-265674a1dde7">Functions</a>
 

 

