---
UID: NF:d2d1helper.PixelFormat
title: PixelFormat function
author: windows-sdk-content
description: Creates a D2D1_PIXEL_FORMAT structure.
old-location: direct2d\pixelformat.htm
tech.root: Direct2D
ms.assetid: 97128e07-68c2-40ab-bad1-7b6f599291b9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PixelFormat, PixelFormat function [Direct2D], d2d1helper/PixelFormat, direct2d.pixelformat
ms.topic: function
req.header: d2d1helper.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D2d1.lib
req.dll: D2d1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - D2d1.dll
api_name:
 - PixelFormat
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PixelFormat function


## -description


Creates a  <a href="https://msdn.microsoft.com/e95afd9c-5793-4cb7-bcb8-aae4d28b6532">D2D1_PIXEL_FORMAT</a> structure.


## -parameters




### -param dxgiFormat [in]

Type: <b><a href="http://msdn.microsoft.com/en-us/library/bb173059(VS.85).aspx">DXGI_FORMAT</a></b>

A value that specifies the size and arrangement of channels in each pixel. The default value is <a href="http://msdn.microsoft.com/en-us/library/bb173059(VS.85).aspx">DXGI_FORMAT_UNKNOWN</a>.


### -param alphaMode [in]

Type: <b><a href="https://msdn.microsoft.com/f1b1e735-2e89-4dc1-9fee-dfb4626ef453">ALPHA_MODE</a></b>

A value that specifies whether the alpha channel is using premultiplied alpha or  straight alpha, or whether it should be ignored and considered opaque. The default value is <a href="https://msdn.microsoft.com/f1b1e735-2e89-4dc1-9fee-dfb4626ef453">D2D1_ALPHA_MODE_UNKNOWN</a>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/e95afd9c-5793-4cb7-bcb8-aae4d28b6532">D2D1_PIXEL_FORMAT</a></b>

A structure that  contains the data format and alpha mode for a bitmap or render target.  




## -see-also




<a href="https://msdn.microsoft.com/09b1f9c6-1780-4733-ac22-9e8c21466b67">Supported Pixel Formats and Alpha Modes</a>
 

 

