---
UID: NF:d2d1_3.ID2D1Ink.StreamAsGeometry(ID2D1InkStyle,const D2D1_MATRIX_3X2_F &,ID2D1SimplifiedGeometrySink)
title: ID2D1Ink::StreamAsGeometry(ID2D1InkStyle,const D2D1_MATRIX_3X2_F &,ID2D1SimplifiedGeometrySink) (d2d1_3.h)
author: windows-sdk-content
description: Retrieves a geometric representation of this ink object.
old-location: direct2d\id2d1ink_streamasgeometry_4.htm
tech.root: Direct2D
ms.assetid: CCAC4872-47FF-4E0D-BE43-2DF6D5882E26
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: ID2D1Ink interface [Direct2D],StreamAsGeometry method, ID2D1Ink.StreamAsGeometry, ID2D1Ink.StreamAsGeometry(ID2D1InkStyle,const D2D1_MATRIX_3X2_F &,ID2D1SimplifiedGeometrySink), ID2D1Ink::StreamAsGeometry, ID2D1Ink::StreamAsGeometry(ID2D1InkStyle,const D2D1_MATRIX_3X2_F &,ID2D1SimplifiedGeometrySink), StreamAsGeometry, StreamAsGeometry method [Direct2D], StreamAsGeometry method [Direct2D],ID2D1Ink interface, d2d1_3/ID2D1Ink::StreamAsGeometry, direct2d.id2d1ink_streamasgeometry_4
ms.topic: method
req.header: d2d1_3.h
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
req.lib: D2d1_3.lib
req.dll: D2d1_3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - d2d1_3.dll
api_name:
 - ID2D1Ink.StreamAsGeometry
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID2D1Ink::StreamAsGeometry(ID2D1InkStyle,const D2D1_MATRIX_3X2_F &,ID2D1SimplifiedGeometrySink)


## -description


Retrieves a geometric representation of this ink object.


## -parameters




### -param inkStyle [in, optional]

Type: <b><a href="https://msdn.microsoft.com/03853FA5-1377-42FB-A4C2-50069DDF6E2D">ID2D1InkStyle</a>*</b>

The ink style to be used in determining the geometric representation.


### -param worldTransform [ref]

Type: <b>const <a href="https://msdn.microsoft.com/f05d7555-6482-4eea-950f-7b443892cc1f">D2D1_MATRIX_3X2_F</a></b>

The world transform to be used in determining the geometric representation.


### -param geometrySink [in]

Type: <b><a href="https://msdn.microsoft.com/cf877a25-7b9f-4db0-ac53-b4a350795a86">ID2D1SimplifiedGeometrySink</a>*</b>

The geometry sink to which the geometry representation will be streamed.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/4B6DD4C2-8E91-4AEA-AFB5-21B4FD13F75A">ID2D1Ink</a>
 

 

