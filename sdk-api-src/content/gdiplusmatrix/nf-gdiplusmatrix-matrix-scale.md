---
UID: NF:gdiplusmatrix.Matrix.Scale
title: Matrix::Scale (gdiplusmatrix.h)
author: windows-sdk-content
description: The Matrix::Scale method updates this matrix with the product of itself and a scaling matrix.
old-location: gdiplus\_gdiplus_CLASS_Matrix_Scale_scaleX_scaleY_order_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\matrixclass\matrixmethods\scale.htm
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: Matrix class [GDI+],Scale method, Matrix.Scale, Matrix::Scale, Scale, Scale method [GDI+], Scale method [GDI+],Matrix class, _gdiplus_CLASS_Matrix_Scale_scaleX_scaleY_order_, gdiplus._gdiplus_CLASS_Matrix_Scale_scaleX_scaleY_order_
ms.topic: method
req.header: gdiplusmatrix.h
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
 - Matrix.Scale
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Matrix::Scale


## -description


The <b>Matrix::Scale</b> method updates this matrix with the product of itself and a scaling matrix.


## -parameters




### -param scaleX [in]

Type: <b>REAL</b>

Real number that specifies the horizontal scale factor. 


### -param scaleY [in]

Type: <b>REAL</b>

Real number that specifies the vertical scale factor. 


### -param order [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a></b>

Optional. Element of the <a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a> enumeration that specifies the order of the multiplication. MatrixOrderPrepend specifies that the scaling matrix is on the left, and MatrixOrderAppend specifies that the scaling matrix is on the right. The default value is MatrixOrderPrepend. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms536395(v=VS.85).aspx">Global and Local Transformations</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534475(v=VS.85).aspx">Matrix</a>



<a href="https://msdn.microsoft.com/en-us/library/ms536397(v=VS.85).aspx">Matrix Representation of Transformations</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535308(v=VS.85).aspx">Matrix::Multiply</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535312(v=VS.85).aspx">Matrix::Rotate</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535313(v=VS.85).aspx">Matrix::RotateAt</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535316(v=VS.85).aspx">Matrix::Shear</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535317(v=VS.85).aspx">Matrix::Translate</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533810(v=VS.85).aspx">Transformations</a>
 

 

