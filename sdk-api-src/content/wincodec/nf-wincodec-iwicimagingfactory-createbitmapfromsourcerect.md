---
UID: NF:wincodec.IWICImagingFactory.CreateBitmapFromSourceRect
title: IWICImagingFactory::CreateBitmapFromSourceRect (wincodec.h)
author: windows-sdk-content
description: Creates an IWICBitmap from a specified rectangle of an IWICBitmapSource.
old-location: wic\_wic_codec_iwicimagingfactory_createbitmapfromsourcerect.htm
tech.root: wic
ms.assetid: 54111643-523a-4197-b7e9-ee0efeae5b88
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CreateBitmapFromSourceRect, CreateBitmapFromSourceRect method [Windows Imaging Component], CreateBitmapFromSourceRect method [Windows Imaging Component],IWICImagingFactory interface, IWICImagingFactory interface [Windows Imaging Component],CreateBitmapFromSourceRect method, IWICImagingFactory.CreateBitmapFromSourceRect, IWICImagingFactory::CreateBitmapFromSourceRect, _wic_codec_iwicimagingfactory_createbitmapfromsourcerect, wic._wic_codec_iwicimagingfactory_createbitmapfromsourcerect, wincodec/IWICImagingFactory::CreateBitmapFromSourceRect
ms.topic: method
req.header: wincodec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wincodec.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Windowscodecs.lib
req.dll: Windowscodecs.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Windowscodecs.dll
api_name:
 - IWICImagingFactory.CreateBitmapFromSourceRect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWICImagingFactory::CreateBitmapFromSourceRect


## -description


Creates an <a href="https://msdn.microsoft.com/15dcc80d-ef58-453d-a57a-348ffc7ddc6b">IWICBitmap</a> from a specified rectangle of an <a href="https://msdn.microsoft.com/abcc84af-6067-4856-8618-fb66aff4255a">IWICBitmapSource</a>.


## -parameters




### -param pIBitmapSource [in]

Type: <b><a href="https://msdn.microsoft.com/abcc84af-6067-4856-8618-fb66aff4255a">IWICBitmapSource</a>*</b>

The <a href="https://msdn.microsoft.com/abcc84af-6067-4856-8618-fb66aff4255a">IWICBitmapSource</a> to create the bitmap from.


### -param x [in]

Type: <b>UINT</b>

The horizontal coordinate of the upper-left corner of the rectangle.


### -param y [in]

Type: <b>UINT</b>

The vertical coordinate of the upper-left corner of the rectangle.


### -param width [in]

Type: <b>UINT</b>

The width of the rectangle and the new bitmap.


### -param height [in]

Type: <b>UINT</b>

The height of the rectangle and the new bitmap.


### -param ppIBitmap [out]

Type: <b><a href="https://msdn.microsoft.com/15dcc80d-ef58-453d-a57a-348ffc7ddc6b">IWICBitmap</a>**</b>

A pointer that receives a pointer to the new bitmap.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Providing a rectangle that is larger than the source will produce undefined results.

This method always creates a separate copy of the source image, similar to the cache option <a href="https://msdn.microsoft.com/121d394d-e818-44c5-bf44-3b01df61c780">WICBitmapCacheOnLoad</a>.



