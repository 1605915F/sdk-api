---
UID: NF:gdiplusheaders.Region.Exclude(IN const GraphicsPath)
title: Region::Exclude(IN const GraphicsPath)
author: windows-sdk-content
description: The Region::Exclude method updates this region to the portion of itself that does not intersect the specified path's interior.
old-location: gdiplus\_gdiplus_CLASS_Region_Exclude_path_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\regionclass\regionmethods\regionexcludemethods\exclude.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Exclude, Exclude method [GDI+], Exclude method [GDI+],Region class, Region class [GDI+],Exclude method, Region.Exclude, Region.Exclude(IN const GraphicsPath), Region.Exclude(const GraphicsPath*), Region::Exclude, Region::Exclude(IN const GraphicsPath), _gdiplus_CLASS_Region_Exclude_path_, gdiplus._gdiplus_CLASS_Region_Exclude_path_
ms.topic: method
req.header: gdiplusheaders.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
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
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gdiplus.dll
api_name:
 - Region.Exclude
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Region::Exclude(IN const GraphicsPath)


## -description


The <b>Region::Exclude</b> method updates this region to the portion of itself that does not intersect the specified path's interior.


## -parameters




### -param path [in]

Type: <b>const <a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>*</b>

Pointer to a <a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a> object that specifies the path to use to update this 
					<a href="https://msdn.microsoft.com/2972b879-7d2f-4cad-b17d-670125f43691">Region</a>object. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Ok</a>, which is an element of the <b>Status</b> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>



<a href="https://msdn.microsoft.com/2972b879-7d2f-4cad-b17d-670125f43691">Region</a>



<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a>
 

 

