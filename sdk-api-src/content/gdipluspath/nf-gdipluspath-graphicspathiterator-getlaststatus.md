---
UID: NF:gdipluspath.GraphicsPathIterator.GetLastStatus
title: GraphicsPathIterator::GetLastStatus
author: windows-sdk-content
description: The GraphicsPathIterator::GetLastStatus method returns a value that indicates the nature of this GraphicsPathIterator object's most recent method failure.
old-location: gdiplus\_gdiplus_CLASS_GraphicsPathIterator_GetLastStatus_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicspathiteratorclass\graphicspathiteratormethods\getlaststatus_19.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLastStatus, GetLastStatus method [GDI+], GetLastStatus method [GDI+],GraphicsPathIterator class, GraphicsPathIterator class [GDI+],GetLastStatus method, GraphicsPathIterator.GetLastStatus, GraphicsPathIterator::GetLastStatus, _gdiplus_CLASS_GraphicsPathIterator_GetLastStatus_, gdiplus._gdiplus_CLASS_GraphicsPathIterator_GetLastStatus_
ms.topic: method
req.header: gdipluspath.h
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
 - GraphicsPathIterator.GetLastStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# GraphicsPathIterator::GetLastStatus


## -description


The <b>GraphicsPathIterator::GetLastStatus</b> method returns a value that indicates the nature of this <a href="https://msdn.microsoft.com/en-us/library/ms534458(v=VS.85).aspx">GraphicsPathIterator</a> object's most recent method failure.


## -parameters






## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

The <b>GraphicsPathIterator::GetLastStatus</b> method returns an element of the <a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If no methods invoked on this <a href="https://msdn.microsoft.com/en-us/library/ms534458(v=VS.85).aspx">GraphicsPathIterator</a> object have failed since the previous call to <b>GetLastStatus</b>, then <b>GetLastStatus</b> returns Ok.

If at least one method invoked on this <a href="https://msdn.microsoft.com/en-us/library/ms534458(v=VS.85).aspx">GraphicsPathIterator</a> object has failed since the previous call to <b>GraphicsPathIterator::GetLastStatus</b> then <b>GraphicsPathIterator::GetLastStatus</b> returns a value that indicates the nature of the most recent failure.




## -remarks



You can call <b>GraphicsPathIterator::GetLastStatus</b> immediately after constructing a <a href="https://msdn.microsoft.com/en-us/library/ms534458(v=VS.85).aspx">GraphicsPathIterator</a> object to determine whether the constructor succeeded.

The first time you call the <b>GraphicsPathIterator::GetLastStatus</b> method of a <a href="https://msdn.microsoft.com/en-us/library/ms534458(v=VS.85).aspx">GraphicsPathIterator</a> object, it returns Ok if the constructor succeeded and all methods invoked so far on the <b>GraphicsPathIterator</b> object succeeded. Otherwise, it returns a value that indicates the nature of the most recent failure.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms533805(v=VS.85).aspx">Constructing and Drawing Paths</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534458(v=VS.85).aspx">GraphicsPathIterator</a>



<a href="https://msdn.microsoft.com/en-us/library/ms536370(v=VS.85).aspx">Paths</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a>
 

 

