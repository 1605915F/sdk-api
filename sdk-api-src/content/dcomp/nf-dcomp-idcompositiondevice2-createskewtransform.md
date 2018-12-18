---
UID: NF:dcomp.IDCompositionDevice2.CreateSkewTransform
title: IDCompositionDevice2::CreateSkewTransform
author: windows-sdk-content
description: Creates a 2D skew transform object.
old-location: directcomp\idcompositiondevice2_createskewtransform.htm
tech.root: directcomp
ms.assetid: 10700E97-C799-4FC0-8300-B5347CC67AC3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateSkewTransform, CreateSkewTransform method [DirectComposition], CreateSkewTransform method [DirectComposition],IDCompositionDevice2 interface, IDCompositionDevice2 interface [DirectComposition],CreateSkewTransform method, IDCompositionDevice2.CreateSkewTransform, IDCompositionDevice2::CreateSkewTransform, dcomp/IDCompositionDevice2::CreateSkewTransform, directcomp.idcompositiondevice2_createskewtransform
ms.topic: method
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps only]
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
 - IDCompositionDevice2.CreateSkewTransform
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice2::CreateSkewTransform


## -description


Creates a 2D skew transform object.


## -parameters




### -param skewTransform [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh449057(v=VS.85).aspx">IDCompositionSkewTransform</a>**</b>

The new 2D skew transform object. This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



A new 2D skew transform object has a static value of zero for the AngleX, AngleY, CenterX, and CenterY properties.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn280354(v=VS.85).aspx">IDCompositionDevice2</a>



<a href="https://msdn.microsoft.com/DA3CBBB6-DB0A-4FCE-9DAC-7A767783A18D">IDCompositionVisual::SetTransform</a>
 

 

