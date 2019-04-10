---
UID: NF:gdiplusgraphics.Graphics.FromImage
title: Graphics::FromImage (gdiplusgraphics.h)
author: windows-sdk-content
description: The Graphics::FromImage method creates a Graphicsobject that is associated with a specified Image object.
old-location: gdiplus\_gdiplus_CLASS_Graphics_FromImage_image_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\fromimage.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: FromImage, FromImage method [GDI+], FromImage method [GDI+],Graphics class, Graphics class [GDI+],FromImage method, Graphics.FromImage, Graphics::FromImage, _gdiplus_CLASS_Graphics_FromImage_image_, gdiplus._gdiplus_CLASS_Graphics_FromImage_image_
ms.topic: method
req.header: gdiplusgraphics.h
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
 - Graphics.FromImage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Graphics::FromImage


## -description


The <b>Graphics::FromImage</b> method creates a 
			<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>object that is associated with a specified 
			<a href="https://msdn.microsoft.com/en-us/library/ms534462(v=VS.85).aspx">Image</a> object.


## -parameters




### -param image [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534462(v=VS.85).aspx">Image</a>*</b>

Pointer to an 
					<a href="https://msdn.microsoft.com/en-us/library/ms534462(v=VS.85).aspx">Image</a> object that will be associated with the new 
					<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>object. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>*</b>
</strong>

This method returns a pointer to the new 
						<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>object.




## -remarks



This method fails if the 
				<a href="https://msdn.microsoft.com/en-us/library/ms534462(v=VS.85).aspx">Image</a> object is based on a metafile that was opened for reading. The 
				<a href="https://msdn.microsoft.com/en-us/library/ms535411(v=VS.85).aspx">Image::Image(filename, useEmbeddedColorManagement)</a> and 
				<a href="https://msdn.microsoft.com/en-us/library/ms535285(v=VS.85).aspx">Metafile::Metafile(filename)</a> constructors open a metafile for reading. To open a metafile for recording, use a 
				<a href="https://msdn.microsoft.com/en-us/library/ms534477(v=VS.85).aspx">Metafile</a> constructor that receives a device context handle.

This method also fails if the image has one of the following pixel formats: 

<ul>
<li><b>PixelFormatUndefined</b></li>
<li><b>PixelFormatDontCare</b></li>
<li><b>PixelFormat1bppIndexed</b></li>
<li><b>PixelFormat4bppIndexed</b></li>
<li><b>PixelFormat8bppIndexed</b></li>
<li><b>PixelFormat16bppGrayScale</b></li>
<li><b>PixelFormat16bppARGB1555</b></li>
</ul>

#### Examples



The following example calls the <b>Graphics::FromImage</b> method to create a 
						<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>object that is associated with an 
						<a href="https://msdn.microsoft.com/en-us/library/ms534462(v=VS.85).aspx">Image</a> object. The call to 
						<a href="https://msdn.microsoft.com/en-us/library/ms535969(v=VS.85).aspx">Graphics::FillEllipse</a>	does not paint on the display device; instead, it alters the bitmap of the 
						<b>Image</b> object. The call to 
						<a href="https://msdn.microsoft.com/en-us/library/ms536030(v=VS.85).aspx">Graphics::DrawImage</a> displays the altered bitmap.


```cpp
VOID Example_FromImage(HDC hdc)
{
   Graphics graphics(hdc);

   // Create an Image object from a PNG file.
   Image image(L"Mosaic.png");

   // Create a Graphics object that is associated with the image.
   Graphics* imageGraphics = Graphics::FromImage(&image);
   
   // Alter the image.
   SolidBrush brush(Color(255, 0, 0, 255));
   imageGraphics->FillEllipse(&brush, 10, 40, 100, 50);

   // Draw the altered image.
   graphics.DrawImage(&image, 30, 20);
   
   delete imageGraphics;
}
```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms536339(v=VS.85).aspx">Changes in the Programming Model</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535778(v=VS.85).aspx">FromHDC Methods</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534453(v=VS.85).aspx">Graphics</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535632(v=VS.85).aspx">Graphics Constructors</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535694(v=VS.85).aspx">Graphics::FromHWND</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535709(v=VS.85).aspx">Graphics::GetHDC</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533815(v=VS.85).aspx">Using Images, Bitmaps, and Metafiles</a>
 

 

