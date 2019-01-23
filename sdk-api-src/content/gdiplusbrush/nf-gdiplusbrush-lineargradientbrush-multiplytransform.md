---
UID: NF:gdiplusbrush.LinearGradientBrush.MultiplyTransform
title: LinearGradientBrush::MultiplyTransform
author: windows-sdk-content
description: The LinearGradientBrush::MultiplyTransform method updates this brush's transformation matrix with the product of itself and another matrix.
old-location: gdiplus\_gdiplus_CLASS_LinearGradientBrush_MultiplyTransform_matrix_order_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\lineargradientbrushclass\lineargradientbrushmethods\multiplytransform_12matrix_order.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: LinearGradientBrush class [GDI+],MultiplyTransform method, LinearGradientBrush.MultiplyTransform, LinearGradientBrush::MultiplyTransform, MultiplyTransform, MultiplyTransform method [GDI+], MultiplyTransform method [GDI+],LinearGradientBrush class, _gdiplus_CLASS_LinearGradientBrush_MultiplyTransform_matrix_order_, gdiplus._gdiplus_CLASS_LinearGradientBrush_MultiplyTransform_matrix_order_
ms.topic: method
req.header: gdiplusbrush.h
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
 - LinearGradientBrush.MultiplyTransform
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# LinearGradientBrush::MultiplyTransform


## -description


The <b>LinearGradientBrush::MultiplyTransform</b> method updates this brush's transformation matrix with the product of itself and another matrix.


## -parameters




### -param matrix [in]

Type: <b>const <a href="https://msdn.microsoft.com/en-us/library/ms534475(v=VS.85).aspx">Matrix</a>*</b>

Pointer to a matrix to be multiplied by the brush's current transformation matrix. 


### -param order [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a></b>

Optional. Element of the <a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a> enumeration that specifies the order of the multiplication. MatrixOrderPrepend specifies that the passed matrix is on the left, and MatrixOrderAppend specifies that the passed matrix is on the right. The default value is MatrixOrderPrepend. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/en-us/library/ms534175(v=VS.85).aspx">Status</a> enumeration.




## -remarks



A single 3
				×3 matrix can store any sequence of affine transformations. If you have several 3
				×3 matrices, each of which represents an affine transformation, the product of those matrices is a single 3
				×3 matrix that represents the entire sequence of transformations. The transformation represented by that product is called a composite transformation. For example, suppose matrix R represents a rotation, and matrix T represents a translation. If matrix M is the product RT, then matrix M represents a composite transformation: first rotate, then translate.

The order of matrix multiplication is important. In general, the matrix product RT is not the same as the matrix product TR. In the example given in the previous paragraph, the composite transformation represented by RT (first rotate, then translate) is not the same as the composite transformation represented by TR (first translate, then rotate).


#### Examples



The following example creates a linear gradient brush and uses it to fill a rectangle. Next, the code sets the brush's transformation matrix, fills a rectangle with the transformed brush, modifies the brush's transformation matrix, and again fills a rectangle with the transformed brush.


```cpp
VOID Example_MultTrans(HDC hdc)
{
   Graphics myGraphics(hdc);

   Matrix S(2, 0, 0, 1, 0, 0);   // horizontal doubling
   Matrix T(1, 0, 0, 1, 50, 0);  // horizontal translation of 50 units

   LinearGradientBrush linGrBrush(
      Rect(0, 0, 200, 100),
      Color(255, 255, 0, 0),     // red
      Color(255, 0, 0, 255),     // blue
      LinearGradientModeHorizontal);

   // Fill a large area with the gradient brush (no transformation).
   myGraphics.FillRectangle(&linGrBrush, 0, 0, 800, 100);

   // Apply the scaling transformation.
   linGrBrush.SetTransform(&S);

   // Fill a large area with the scaled gradient brush.
   myGraphics.FillRectangle(&linGrBrush, 0, 150, 800, 100);

   // Form a composite transformation: first scale, then translate.
   linGrBrush.MultiplyTransform(&T, MatrixOrderAppend);

   // Fill a large area with the scaled and translated gradient brush.
   myGraphics.FillRectangle(&linGrBrush, 0, 300, 800, 100);
}
```





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms536356(v=VS.85).aspx">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533806(v=VS.85).aspx">Filling Shapes with a Gradient Brush</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534473(v=VS.85).aspx">LinearGradientBrush</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535340(v=VS.85).aspx">LinearGradientBrush::RotateTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535341(v=VS.85).aspx">LinearGradientBrush::ScaleTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms535350(v=VS.85).aspx">LinearGradientBrush::TranslateTransform</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534475(v=VS.85).aspx">Matrix</a>



<a href="https://msdn.microsoft.com/en-us/library/ms536397(v=VS.85).aspx">Matrix Representation of Transformations</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534149(v=VS.85).aspx">MatrixOrder</a>



<a href="https://msdn.microsoft.com/en-us/library/ms534495(v=VS.85).aspx">Rect</a>



<a href="https://msdn.microsoft.com/en-us/library/ms533810(v=VS.85).aspx">Transformations</a>
 

 

