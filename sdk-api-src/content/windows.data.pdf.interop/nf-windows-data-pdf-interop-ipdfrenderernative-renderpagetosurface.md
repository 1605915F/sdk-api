---
UID: NF:windows.data.pdf.interop.IPdfRendererNative.RenderPageToSurface
title: IPdfRendererNative::pdf (windows.data.pdf.interop.h)
author: windows-sdk-content
description: Outputs a single page of a Portable Document Format (PDF) file to a Microsoft DirectX image-data object.
old-location: winrt\ipdfrenderernative_renderpagetosurface.htm
tech.root: WinRT
ms.assetid: d4688c23-0122-40a7-908e-793c3f03fb37
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IPdfRendererNative interface [Windows Runtime],RenderPageToSurface method, IPdfRendererNative.RenderPageToSurface, IPdfRendererNative.pdf, IPdfRendererNative::RenderPageToSurface, IPdfRendererNative::pdf, RenderPageToSurface, RenderPageToSurface method [Windows Runtime], RenderPageToSurface method [Windows Runtime],IPdfRendererNative interface, windows/IPdfRendererNative::RenderPageToSurface, winrt.ipdfrenderernative_renderpagetosurface
ms.topic: method
req.header: windows.data.pdf.interop.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [UWP apps only]
req.target-min-winversvr: Windows Server 2012 R2 [UWP apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Windows.data.pdf.interop.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Windows.data.pdf.lib
req.dll: Windows.Data.Pdf.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Windows.Data.Pdf.dll
api_name:
 - IPdfRendererNative.RenderPageToSurface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPdfRendererNative::pdf


## -description


Outputs a single page of a Portable Document Format (PDF) file to a Microsoft DirectX image-data object.


## -parameters




### -param pdfPage [in]

The <b>IPdfPage</b> interface as an instance of the <a href="https://msdn.microsoft.com/85bf8d83-8c70-472f-8762-709fddaf3222">PdfPage</a> class,  type-casted to the <b>IUnknown</b> interface, representing the page to be output.


### -param pSurface [in]

An instance of the target image-data object.


### -param offset [in]

An x- and y-coordinate offset within the target image-data object to output the page.


### -param pRenderParams [in, optional]

A set of page output properties, such as rendering only a portion of the page, rendering a scaled version of the page, setting the page's background color, and whether the page is shown in high contrast mode. 

Provide a null pointer for this parameter to specify default page output properties. For the list of defaults, see <a href="https://msdn.microsoft.com/1B2F12FB-E053-4B79-B71D-E66D7A6E5054">PDF_RENDER_PARAMS</a>.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The page output operation succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/96a00afb-e957-4e49-8f30-d6a3d639680f">IPdfRendererNative</a>
 

 

