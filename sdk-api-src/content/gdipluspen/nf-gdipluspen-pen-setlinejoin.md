---
UID: NF:gdipluspen.Pen.SetLineJoin
title: Pen::SetLineJoin (gdipluspen.h)
author: windows-sdk-content
description: The Pen::SetLineJoin method sets the line join for this Pen object.
old-location: gdiplus\_gdiplus_CLASS_Pen_SetLineJoin_lineJoin_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\penclass\penmethods\setlinejoin.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Pen class [GDI+],SetLineJoin method, Pen.SetLineJoin, Pen::SetLineJoin, SetLineJoin, SetLineJoin method [GDI+], SetLineJoin method [GDI+],Pen class, _gdiplus_CLASS_Pen_SetLineJoin_lineJoin_, gdiplus._gdiplus_CLASS_Pen_SetLineJoin_lineJoin_
ms.topic: method
req.header: gdipluspen.h
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
 - Pen.SetLineJoin
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
ms.custom: 19H1
---

# Pen::SetLineJoin


## -description


The <b>Pen::SetLineJoin</b> method sets the line join for this 
			<a href="https://msdn.microsoft.com/en-us/library/ms534485(v=VS.85).aspx">Pen</a> object.


## -parameters




### -param lineJoin [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534148(v=VS.85).aspx">LineJoin</a></b>

Element of the 
					<a href="https://msdn.microsoft.com/en-us/library/ms534148(v=VS.85).aspx">LineJoin</a> enumeration that specifies the join style used at the end of a line segment that meets another line segment. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms533853(v=VS.85).aspx">Joining Lines</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534146(v=VS.85).aspx">LineCap</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534485(v=VS.85).aspx">Pen</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535029(v=VS.85).aspx">Pen::GetEndCap</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535034(v=VS.85).aspx">Pen::GetStartCap</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535051(v=VS.85).aspx">Pen::SetEndCap</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535052(v=VS.85).aspx">Pen::SetLineCap</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535055(v=VS.85).aspx">Pen::SetStartCap</a>



<a href="https://msdn.microsoft.com/en-us/library/ms536372(v=VS.85).aspx">Pens, Lines, and Rectangles</a>
 

 

