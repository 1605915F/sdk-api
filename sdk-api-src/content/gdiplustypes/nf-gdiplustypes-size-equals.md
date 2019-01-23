---
UID: NF:gdiplustypes.Size.Equals
title: Size::Equals
author: windows-sdk-content
description: The Size::Equals method determines whether two Size objects are equal.
old-location: gdiplus\_gdiplus_CLASS_Size_Equals_sz_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\sizeclass\sizemethods\equals_53sz.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Equals, Equals method [GDI+], Equals method [GDI+],Size class, Size class [GDI+],Equals method, Size.Equals, Size::Equals, _gdiplus_CLASS_Size_Equals_sz_, gdiplus._gdiplus_CLASS_Size_Equals_sz_
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
 - Size.Equals
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Size::Equals


## -description


The <b>Size::Equals</b> method determines whether two 
			<a href="https://msdn.microsoft.com/en-us/library/ms534504(v=VS.85).aspx">Size</a> objects are equal.


## -parameters




### -param sz [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/ms534504(v=VS.85).aspx">Size</a></b>

Reference to a 
					<a href="https://msdn.microsoft.com/en-us/library/ms534504(v=VS.85).aspx">Size</a> object that is compared to this 
					<b>Size</b> object. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the 
						<b>Width</b> and 
						<b>Height</b>  data members of the two 
						<a href="https://msdn.microsoft.com/en-us/library/ms534504(v=VS.85).aspx">Size</a> objects are equal, this method returns <b>TRUE</b>; otherwise, it returns <b>FALSE</b>.




## -remarks



Two 
				<a href="https://msdn.microsoft.com/en-us/library/ms534504(v=VS.85).aspx">Size</a> objects are defined as equal if the 
				<b>Width</b> and 
				<b>Height</b>  data members are equal.


#### Examples



The following example creates a 
						<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a> object, gets the size of the rectangle, and determines whether the rectangles are equal.


```cpp
Rect rect(50, 30, 200, 100);
Size desiredSize(200, 100);
Size rectSize;

// Get the size of the rectangle.
rect.GetSize(&rectSize);

if(rectSize.Equals(desiredSize))
{
   // The rectangle has the desired size.
} 
```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534504(v=VS.85).aspx">Size</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534506(v=VS.85).aspx">SizeF</a>
 

 

