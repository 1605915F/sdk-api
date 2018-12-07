---
UID: NF:d2d1.ID2D1Geometry.FillContainsPoint
title: ID2D1Geometry::FillContainsPoint
author: windows-sdk-content
description: Indicates whether the area filled by the geometry would contain the specified point given the specified flattening tolerance.
old-location: direct2d\ID2D1Geometry_FillContainsPoint_D2D_POINT_2F_ptr_D2D_MATRIX_3X2_F_FLOAT_ptr_BOOL.htm
tech.root: direct2d
ms.assetid: 2f54b538-afa5-4dd9-80e3-5441c0e7bddf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FillContainsPoint, FillContainsPoint method [Direct2D], FillContainsPoint method [Direct2D],ID2D1Geometry interface, ID2D1Geometry interface [Direct2D],FillContainsPoint method, ID2D1Geometry.FillContainsPoint, ID2D1Geometry::FillContainsPoint, ID2D1Geometry::FillContainsPoint(D2D1_POINT_2F,const D2D1_MATRIX_3X2_F,FLOAT,BOOL), d2d1/ID2D1Geometry::FillContainsPoint, direct2d.ID2D1Geometry_FillContainsPoint_D2D_POINT_2F_ptr_D2D_MATRIX_3X2_F_FLOAT_ptr_BOOL
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1.h
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
 - COM
api_location:
 - D2d1.dll
api_name:
 - ID2D1Geometry.FillContainsPoint
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1Geometry::FillContainsPoint


## -description


Indicates whether the area filled by the geometry would contain the specified point given the specified flattening tolerance.




## -parameters




### -param point

Type: <b><a href="https://msdn.microsoft.com/b317ae75-d738-4e1a-bcd1-adf3e95b197e">D2D1_POINT_2F</a></b>

The point to test.



### -param worldTransform [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/f05d7555-6482-4eea-950f-7b443892cc1f">D2D1_MATRIX_3X2_F</a>*</b>

The transform to apply to the geometry prior to testing for containment, or <b>NULL</b>.


### -param flatteningTolerance

Type: <b>FLOAT</b>

The numeric accuracy with which the precise geometric path and path intersection is calculated. Points missing the fill by less than the tolerance are still considered inside.  Smaller values produce more accurate results but cause slower execution. 



### -param contains [out]

Type: <b>BOOL*</b>

When this method returns, contains a <b>BOOL</b> value that is <b>TRUE</b> if the area filled by the geometry contains <i>point</i>; otherwise, <b>FALSE</b>.
You must allocate storage for this parameter.


## -returns



Type: <b><a href="a9046ed2-bfb2-4d56-a719-2824afce59ac">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/be4ab801-64f6-48f9-8f62-d0492cc438b1">ID2D1Geometry</a>
 

 

