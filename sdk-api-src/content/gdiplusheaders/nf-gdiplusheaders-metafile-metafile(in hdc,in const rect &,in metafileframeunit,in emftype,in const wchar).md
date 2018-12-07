---
UID: NF:gdiplusheaders.Metafile.Metafile(IN HDC,IN const Rect &,IN MetafileFrameUnit,IN EmfType,IN const WCHAR)
title: Metafile::Metafile(IN HDC,IN const Rect &,IN MetafileFrameUnit,IN EmfType,IN const WCHAR)
author: windows-sdk-content
description: Creates a Metafile::Metafile object for recording.
old-location: gdiplus\_gdiplus_CLASS_Metafile_Metafile_HDC_referenceHdc_Rect_frameRect_MetafileFrameUnit_frameUnit_EmfType.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\metafileclass\metafileconstructors\metafile_93hdcreferencehdc_rectampframerect_metaf.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Metafile, Metafile class [GDI+],Metafile constructor, Metafile constructor [GDI+], Metafile constructor [GDI+],Metafile class, Metafile.Metafile, Metafile.Metafile(HDC,const Rect&,MetafileFrameUnit,EmfType,const WCHAR*), Metafile.Metafile(IN HDC,IN const Rect &,IN MetafileFrameUnit,IN EmfType,IN const WCHAR), Metafile::Metafile, Metafile::Metafile(IN HDC,IN const Rect &,IN MetafileFrameUnit,IN EmfType,IN const WCHAR), _gdiplus_CLASS_Metafile_Metafile_HDC_referenceHdc_Rect_frameRect_MetafileFrameUnit_frameUnit_EmfType, gdiplus._gdiplus_CLASS_Metafile_Metafile_HDC_referenceHdc_Rect_frameRect_MetafileFrameUnit_frameUnit_EmfType
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
 - Metafile.Metafile
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Metafile::Metafile(IN HDC,IN const Rect &,IN MetafileFrameUnit,IN EmfType,IN const WCHAR)


## -description


Creates a <b>Metafile::Metafile</b> object for recording.


## -parameters




### -param referenceHdc [in]

Type: <b>HDC</b>

Windows handle to a device context that contains attributes of the display device that is used to record the metafile. 


### -param frameRect [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/9b995615-3ea1-488d-8960-90add719c3f9">Rect</a></b>

Reference to a rectangle that bounds the metafile display. 


### -param frameUnit [in]

Type: <b><a href="https://msdn.microsoft.com/34b1a9cf-7979-4371-b5a8-db03ea5eb010">MetafileFrameUnit</a></b>

Optional. Element of the <a href="https://msdn.microsoft.com/34b1a9cf-7979-4371-b5a8-db03ea5eb010">MetafileFrameUnit</a> enumeration that specifies the unit of measure for <i>frameRect</i>. The default value is <a href="https://msdn.microsoft.com/34b1a9cf-7979-4371-b5a8-db03ea5eb010">MetafileFrameUnitGdi</a>. 


### -param type [in]

Type: <b><a href="https://msdn.microsoft.com/985c412f-10ba-4ce9-b0e1-89f5b643c22a">EmfType</a></b>

Optional. Element of the <a href="https://msdn.microsoft.com/985c412f-10ba-4ce9-b0e1-89f5b643c22a">EmfType</a> enumeration that specifies the type of metafile that will be recorded. The default value is <a href="https://msdn.microsoft.com/985c412f-10ba-4ce9-b0e1-89f5b643c22a">EmfTypeEmfPlusDual</a>. 


### -param description [in]

Type: <b>const WCHAR*</b>

Optional. Pointer to a wide-character string that specifies the descriptive name of the metafile. The default value is <b>NULL</b>. 


## -remarks



When recording to a file, the file must be writable, and Windows GDI+ must be able to obtain an exclusive lock on the file.




## -see-also




<a href="https://msdn.microsoft.com/985c412f-10ba-4ce9-b0e1-89f5b643c22a">EmfType</a>



<a href="https://msdn.microsoft.com/79b8df1b-6fc5-455b-9d08-57d64bf6bffa">Loading and Displaying Metafiles</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534477(v=VS.85).aspx">Metafile</a>



<a href="https://msdn.microsoft.com/34b1a9cf-7979-4371-b5a8-db03ea5eb010">MetafileFrameUnit</a>



<a href="https://msdn.microsoft.com/a9f9bac4-f3c7-44a1-9f0f-59ff1a27b077">Metafiles</a>



<a href="https://msdn.microsoft.com/062de6c2-9f82-415d-860e-2d1afd2ac027">Recording Metafiles</a>



<a href="https://msdn.microsoft.com/9b995615-3ea1-488d-8960-90add719c3f9">Rect</a>
 

 

