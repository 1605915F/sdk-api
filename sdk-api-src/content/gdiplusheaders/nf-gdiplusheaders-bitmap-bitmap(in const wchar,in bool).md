---
UID: NF:gdiplusheaders.Bitmap.Bitmap(IN const WCHAR,IN BOOL)
title: Bitmap::Bitmap(IN const WCHAR,IN BOOL)
author: windows-sdk-content
description: Creates a Bitmap::Bitmap object based on an image file.
old-location: gdiplus\_gdiplus_CLASS_Bitmap_Bitmap_filename_useIcm_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\bitmapclass\bitmapconstructors\bitmap_56filename_useicm.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Bitmap, Bitmap class [GDI+],Bitmap constructor, Bitmap constructor [GDI+], Bitmap constructor [GDI+],Bitmap class, Bitmap.Bitmap, Bitmap.Bitmap(IN const WCHAR,IN BOOL), Bitmap.Bitmap(const WCHAR*,BOOL), Bitmap::Bitmap, Bitmap::Bitmap(IN const WCHAR,IN BOOL), _gdiplus_CLASS_Bitmap_Bitmap_filename_useIcm_, gdiplus._gdiplus_CLASS_Bitmap_Bitmap_filename_useIcm_
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
 - Bitmap.Bitmap
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Bitmap::Bitmap(IN const WCHAR,IN BOOL)


## -description


Creates a <b>Bitmap::Bitmap</b> object based on an image file.


## -parameters




### -param filename [in]

Type: <b>const WCHAR*</b>

Pointer to a null-terminated string that specifies the path name of the image file. The graphics file formats supported by GDI+ are BMP, GIF, JPEG, PNG, TIFF, Exif, WMF, and EMF. 


### -param useEmbeddedColorManagement [in]

Type: <b>BOOL</b>

Optional. Boolean value that specifies whether the new <b>Bitmap::Bitmap</b> object applies color correction according to color management information that is embedded in the image file. Embedded information can include International Color Consortium (ICC) profiles, gamma values, and chromaticity information. <b>TRUE</b> specifies that color correction is enabled, and <b>FALSE</b> specifies that color correction is not enabled. The default value is <b>FALSE</b>. 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms534420(v=VS.85).aspx">Bitmap</a>



<a href="https://msdn.microsoft.com/9b246a76-e8c0-41b2-9bb2-0df06ebc5563">Bitmap Constructors</a>



<a href="https://msdn.microsoft.com/53f7831d-f5c6-4b0d-89e2-a68380dbb07b">Bitmap::FromFile</a>



<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a>



<a href="https://msdn.microsoft.com/ddde257c-41a6-4f6e-8d81-10d66c60085c">Images, Bitmaps, and Metafiles</a>



<a href="https://msdn.microsoft.com/57e3bf33-5490-4f4a-addf-356ef8f1aeed">Using Images, Bitmaps, and Metafiles</a>
 

 

