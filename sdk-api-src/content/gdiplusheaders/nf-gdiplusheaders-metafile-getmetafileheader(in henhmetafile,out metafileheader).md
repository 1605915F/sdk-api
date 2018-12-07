---
UID: NF:gdiplusheaders.Metafile.GetMetafileHeader(IN HENHMETAFILE,OUT MetafileHeader)
title: Metafile::GetMetafileHeader(IN HENHMETAFILE,OUT MetafileHeader)
author: windows-sdk-content
description: The Metafile::GetMetafileHeader method gets the header.
old-location: gdiplus\_gdiplus_CLASS_Metafile_GetMetafileHeader_hEmf_header_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\metafileclass\metafilemethods\metafilegetmetafileheadermethods\getmetafileheader_41hemf_header.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetMetafileHeader, GetMetafileHeader method [GDI+], GetMetafileHeader method [GDI+],Metafile class, Metafile class [GDI+],GetMetafileHeader method, Metafile.GetMetafileHeader, Metafile.GetMetafileHeader(HENHMETAFILE*,MetafileHeader*), Metafile.GetMetafileHeader(IN HENHMETAFILE,OUT MetafileHeader), Metafile::GetMetafileHeader, Metafile::GetMetafileHeader(IN HENHMETAFILE,OUT MetafileHeader), _gdiplus_CLASS_Metafile_GetMetafileHeader_hEmf_header_, gdiplus._gdiplus_CLASS_Metafile_GetMetafileHeader_hEmf_header_
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - Metafile.GetMetafileHeader
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Metafile::GetMetafileHeader(IN HENHMETAFILE,OUT MetafileHeader)


## -description


The <b>Metafile::GetMetafileHeader</b> method gets the header.


## -parameters




### -param hEmf [in]

Type: <b>HENHMETAFILE*</b>

Window handle to a metafile. 


### -param header [out]

Type: <b><a href="https://msdn.microsoft.com/4ea75699-c3c7-481e-b369-3bdc600b9713">MetafileHeader</a>*</b>

Pointer to a <a href="https://msdn.microsoft.com/4ea75699-c3c7-481e-b369-3bdc600b9713">MetafileHeader</a> object that receives the header, which contains the attributes of the metafile. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns OK, which is an element of the 

						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 

						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/79b8df1b-6fc5-455b-9d08-57d64bf6bffa">Loading and Displaying Metafiles</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534477(v=VS.85).aspx">Metafile</a>



<a href="https://msdn.microsoft.com/538d8376-8922-41ba-abbc-0242474ec4fb">Metafile::GetHENHMETAFILE</a>



<a href="https://msdn.microsoft.com/4ea75699-c3c7-481e-b369-3bdc600b9713">MetafileHeader</a>



<a href="https://msdn.microsoft.com/a9f9bac4-f3c7-44a1-9f0f-59ff1a27b077">Metafiles</a>
 

 

