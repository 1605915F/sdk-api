---
UID: NF:dcomp.IDCompositionRectangleClip.SetLeft(float)
title: IDCompositionRectangleClip::SetLeft(float)
author: windows-sdk-content
description: Changes the value of the Left property of a clip rectangle.
old-location: directcomp\idcompositionrectangleclip_setleft_float.htm
tech.root: directcomp
ms.assetid: 56614B81-3AC7-484C-9049-5E189D1C0B3B
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionRectangleClip interface [DirectComposition],SetLeft method, IDCompositionRectangleClip.SetLeft, IDCompositionRectangleClip.SetLeft(float), IDCompositionRectangleClip::SetLeft, IDCompositionRectangleClip::SetLeft(float), SetLeft, SetLeft method [DirectComposition], SetLeft method [DirectComposition],IDCompositionRectangleClip interface, dcomp/IDCompositionRectangleClip::SetLeft, directcomp.idcompositionrectangleclip_setleft_float
ms.topic: method
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dcomp.lib
req.dll: Dcomp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dcomp.dll
api_name:
 - IDCompositionRectangleClip.SetLeft
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionRectangleClip::SetLeft(float)


## -description


Changes the value of the Left property of a clip rectangle. The Left property specifies the x-coordinate of the upper-left corner of the clip rectangle.
      


## -parameters




### -param left [in]

Type: <b>float</b>

The new value of the Left property, in pixels. This parameter has a numerical limit of -2^21 to 2^21. 
            The API accepts numbers outside of this range, but they are always clamped to this range.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.
            




## -remarks



This method fails if the <i>left</i> parameter is NaN, positive infinity, or negative infinity.

      

If the Left property was previously animated, this method removes the animation and sets the Left property to the specified static value.
      




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh437434(v=VS.85).aspx">IDCompositionRectangleClip</a>
 

 

