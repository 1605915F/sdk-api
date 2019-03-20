---
UID: NF:dcomp.IDCompositionDevice2.CreateTranslateTransform
title: IDCompositionDevice2::CreateTranslateTransform (dcomp.h)
author: windows-sdk-content
description: Creates a 2D translation transform object.
old-location: directcomp\idcompositiondevice2_createtranslatetransform.htm
tech.root: directcomp
ms.assetid: 83800B10-7992-4A3D-B8D6-6872BAEAF7DA
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateTranslateTransform, CreateTranslateTransform method [DirectComposition], CreateTranslateTransform method [DirectComposition],IDCompositionDevice2 interface, IDCompositionDevice2 interface [DirectComposition],CreateTranslateTransform method, IDCompositionDevice2.CreateTranslateTransform, IDCompositionDevice2::CreateTranslateTransform, dcomp/IDCompositionDevice2::CreateTranslateTransform, directcomp.idcompositiondevice2_createtranslatetransform
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
 - IDCompositionDevice2.CreateTranslateTransform
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice2::CreateTranslateTransform


## -description


Creates a 2D translation transform object.


## -parameters




### -param translateTransform [out]

Type: <b><a href="https://msdn.microsoft.com/2215721e-a10d-4c9e-b5b7-1698afa547d8">IDCompositionTranslateTransform</a>**</b>

The new 2D translation transform object. This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



A new 2D translation transform object has a static value of zero for the OffsetX and OffsetY properties.




## -see-also




<a href="https://msdn.microsoft.com/0E5D0AEC-63A3-4A44-9A0B-D1E26789CAB0">IDCompositionDevice2</a>



<a href="https://msdn.microsoft.com/DA3CBBB6-DB0A-4FCE-9DAC-7A767783A18D">IDCompositionVisual::SetTransform</a>
 

 

