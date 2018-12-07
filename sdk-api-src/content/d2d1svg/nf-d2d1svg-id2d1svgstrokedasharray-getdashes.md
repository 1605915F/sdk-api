---
UID: NF:d2d1svg.ID2D1SvgStrokeDashArray.GetDashes
title: ID2D1SvgStrokeDashArray::GetDashes
author: windows-sdk-content
description: Gets dashes from the array.
old-location: direct2d\id2d1svgstrokedasharray_getdashes.htm
tech.root: direct2d
ms.assetid: E5C7A573-3373-4323-8712-93D89B6A53C5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDashes, GetDashes method [Direct2D], GetDashes method [Direct2D],ID2D1SvgStrokeDashArray interface, ID2D1SvgStrokeDashArray interface [Direct2D],GetDashes method, ID2D1SvgStrokeDashArray.GetDashes, ID2D1SvgStrokeDashArray::GetDashes, ID2D1SvgStrokeDashArray::GetDashes(FLOAT,UINT32,UINT32), d2d1svg/ID2D1SvgStrokeDashArray::GetDashes, direct2d.id2d1svgstrokedasharray_getdashes
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1svg.h
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
req.lib: 
req.dll: Direct2d.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - direct2d.dll
api_name:
 - ID2D1SvgStrokeDashArray.GetDashes
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1SvgStrokeDashArray::GetDashes


## -description


Gets dashes from the array.


## -parameters




### -param dashes [out]

Type: <b>FLOAT*</b>

Buffer to contain the dashes.


### -param dashesCount

Type: <b>UINT32</b>

The element count of the array in the dashes argument.


### -param startIndex

Type: <b>UINT32</b>

The index of the first dash to retrieve.


## -returns



Type: <b><a href="455d07e9-52c3-4efb-a9dc-2955cbfd38cc">HRESULT</a></b>

This method returns an HRESULT success or error code.




## -see-also




<a href="https://msdn.microsoft.com/D3C82EC8-4172-48FE-AE8C-5F15BDBBCD30">ID2D1SvgStrokeDashArray</a>
 

 

