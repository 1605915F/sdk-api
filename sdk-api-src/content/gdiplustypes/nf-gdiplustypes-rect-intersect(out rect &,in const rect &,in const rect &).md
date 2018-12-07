---
UID: NF:gdiplustypes.Rect.Intersect(OUT Rect &,IN const Rect &,IN const Rect &)
title: Rect::Intersect(OUT Rect &,IN const Rect &,IN const Rect &)
author: windows-sdk-content
description: The Rect::Intersect method determines the intersection of two rectangles and stores the result in a Rect object.
old-location: gdiplus\_gdiplus_CLASS_Rect_Intersect_c_a_b_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\rectclass\rectmethods\rectintersectmethods\intersect.htm
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: Intersect, Intersect method [GDI+], Intersect method [GDI+],Rect class, Rect class [GDI+],Intersect method, Rect.Intersect, Rect.Intersect(OUT Rect &,IN const Rect &,IN const Rect &), Rect.Intersect(Rect&,const Rect&,const Rect&), Rect::Intersect, Rect::Intersect(OUT Rect &,IN const Rect &,IN const Rect &), _gdiplus_CLASS_Rect_Intersect_c_a_b_, gdiplus._gdiplus_CLASS_Rect_Intersect_c_a_b_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplustypes.h
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
 - Rect.Intersect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- COM
: 
- gdiplustypes.h
: 
- Rect.Intersect
: 
req.product: GDI+ 1.0
---

# Rect::Intersect(OUT Rect &,IN const Rect &,IN const Rect &)


## -description


The <b>Rect::Intersect</b> method determines the intersection of two rectangles and stores the result in a 
			<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a> object.


## -parameters




### -param c [out]

Type: <b>Rect&amp;</b>

Reference to a 
					<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a> object that receives the intersection of the two rectangles. 


### -param a [in]

Type: <b>const Rect&amp;</b>

Reference to one of the two rectangles to be intersected. 


### -param b [in]

Type: <b>const Rect&amp;</b>

Reference to one of the two rectangles to be intersected. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the intersection of the two rectangles is not empty, this method returns <b>TRUE</b>; otherwise, it returns <b>FALSE</b>.




## -see-also




<a href="https://msdn.microsoft.com/b391c256-5165-4c5c-a45a-dee74e32d391">Intersect Methods</a>



<a href="https://msdn.microsoft.com/d91562ab-41e6-4bca-a320-74f490a4f88f">Pens, Lines, and Rectangles</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a>



<a href="https://msdn.microsoft.com/6821442b-d352-48cb-a48a-839105a8c36a">RectF</a>



<a href="https://msdn.microsoft.com/f2e4144f-f2f1-49db-bfdf-ffce3023b4cb">Using a Pen to Draw Lines and Rectangles</a>
 

 

