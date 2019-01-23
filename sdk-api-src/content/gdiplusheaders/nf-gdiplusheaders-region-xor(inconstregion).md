---
UID: NF:gdiplusheaders.Region.Xor(IN const Region)
title: Region::Xor(IN const Region)
author: windows-sdk-content
description: The Region::Xor method updates this region to the nonintersecting portions of itself and another region.
old-location: gdiplus\_gdiplus_CLASS_Region_Xor_region_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\regionclass\regionmethods\regionxormethods\xor_61region.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Region class [GDI+],Xor method, Region.Xor, Region.Xor(IN const Region), Region.Xor(const Region*), Region::Xor, Region::Xor(IN const Region), Xor, Xor method [GDI+], Xor method [GDI+],Region class, _gdiplus_CLASS_Region_Xor_region_, gdiplus._gdiplus_CLASS_Region_Xor_region_
ms.topic: method
req.header: gdiplusheaders.h
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
 - Region.Xor
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Region::Xor(IN const Region)


## -description


The <b>Region::Xor</b> method updates this region to the nonintersecting portions of itself and another region.


## -parameters




### -param region [in]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/ms534501(v=VS.85).aspx">Region</a>*</b>

Pointer to a region to use to update this region. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534501(v=VS.85).aspx">Region</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a>
 

 

