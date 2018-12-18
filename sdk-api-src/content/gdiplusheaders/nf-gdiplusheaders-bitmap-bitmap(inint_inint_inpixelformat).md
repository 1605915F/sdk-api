---
UID: NF:gdiplusheaders.Bitmap.Bitmap(IN INT,IN INT,IN PixelFormat)
title: Bitmap::Bitmap(IN INT,IN INT,IN PixelFormat)
author: windows-sdk-content
description: Creates a Bitmap::Bitmap object of a specified size and pixel format. The pixel data must be provided after the Bitmap::Bitmap object is constructed.
old-location: gdiplus\_gdiplus_CLASS_Bitmap_Bitmap_width_height_format_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\bitmapclass\bitmapconstructors\bitmap_50width_height_format.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Bitmap, Bitmap class [GDI+],Bitmap constructor, Bitmap constructor [GDI+], Bitmap constructor [GDI+],Bitmap class, Bitmap.Bitmap, Bitmap.Bitmap(IN INT,IN INT,IN PixelFormat), Bitmap.Bitmap(INT,INT,PixelFormat), Bitmap::Bitmap, Bitmap::Bitmap(IN INT,IN INT,IN PixelFormat), _gdiplus_CLASS_Bitmap_Bitmap_width_height_format_, gdiplus._gdiplus_CLASS_Bitmap_Bitmap_width_height_format_
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

# Bitmap::Bitmap(IN INT,IN INT,IN PixelFormat)


## -description


Creates a <b>Bitmap::Bitmap</b> object of a specified size and pixel format. The pixel data must be provided after the <b>Bitmap::Bitmap</b> object is constructed.


## -parameters




### -param width [in]

Type: <b>INT</b>

Integer that specifies the width, in pixels, of the bitmap. 


### -param height [in]

Type: <b>INT</b>

Integer that specifies the height, in pixels, of the bitmap. 


### -param format [in]

Type: <b>PixelFormat</b>

Optional. Integer that specifies the pixel format of the bitmap. The 
					<b>PixelFormat</b> data type and constants that represent various pixel formats are defined in Gdipluspixelformats.h. For more information about pixel format constants, see <a href="https://msdn.microsoft.com/362204c5-5dd7-461a-b90b-15826c025689">Image Pixel Format Constants</a>. The default value is PixelFormat32bppARGB. 


## -see-also




<a href="https://msdn.microsoft.com/f9826772-bb8a-4339-9cea-f77637f971b2">Bitmap</a>



<a href="https://msdn.microsoft.com/9b246a76-e8c0-41b2-9bb2-0df06ebc5563">Bitmap Constructors</a>



<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a>



<a href="https://msdn.microsoft.com/362204c5-5dd7-461a-b90b-15826c025689">Image Pixel Format Constants</a>



<a href="https://msdn.microsoft.com/ddde257c-41a6-4f6e-8d81-10d66c60085c">Images, Bitmaps, and Metafiles</a>



<a href="https://msdn.microsoft.com/57e3bf33-5490-4f4a-addf-356ef8f1aeed">Using Images, Bitmaps, and Metafiles</a>
 

 

