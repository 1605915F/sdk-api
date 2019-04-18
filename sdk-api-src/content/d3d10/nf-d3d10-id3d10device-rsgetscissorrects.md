---
UID: NF:d3d10.ID3D10Device.RSGetScissorRects
title: ID3D10Device::RSGetScissorRects (d3d10.h)
author: windows-sdk-content
description: Get the array of scissor rectangles bound to the rasterizer stage.
old-location: direct3d10\id3d10device_rsgetscissorrects.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10device_rsgetscissorrects.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 6718274a-41d0-5a45-3471-07f2693cff9f, ID3D10Device interface [Direct3D 10],RSGetScissorRects method, ID3D10Device.RSGetScissorRects, ID3D10Device::RSGetScissorRects, RSGetScissorRects, RSGetScissorRects method [Direct3D 10], RSGetScissorRects method [Direct3D 10],ID3D10Device interface, d3d10/ID3D10Device::RSGetScissorRects, direct3d10.id3d10device_rsgetscissorrects
ms.topic: method
req.header: d3d10.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D3D10.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D10.lib
 - D3D10.dll
api_name:
 - ID3D10Device.RSGetScissorRects
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10Device::RSGetScissorRects


## -description


Get the array of <a href="https://msdn.microsoft.com/en-us/library/Bb205126(v=VS.85).aspx">scissor rectangles</a> bound to the <a href="https://msdn.microsoft.com/en-us/library/Bb205125(v=VS.85).aspx">rasterizer stage</a>.


## -parameters




### -param NumRects [in, out]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a>*</b>

Number of scissor rectangles to get. If pRects is <b>NULL</b>, this will be filled with the number of scissor rectangles currently bound.


### -param pRects [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb232915(v=VS.85).aspx">D3D10_RECT</a>*</b>

An array of scissor rectangles (see <a href="https://msdn.microsoft.com/en-us/library/Bb232915(v=VS.85).aspx">D3D10_RECT</a>). If NumRects is greater than the number of scissor rects currently bound, then unused members of the array will contain 0.


## -returns



Returns nothing.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Bb173528(v=VS.85).aspx">ID3D10Device Interface</a>
 

 

