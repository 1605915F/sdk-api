---
UID: NF:dcomp.IDCompositionSaturationEffect.SetSaturation(float)
title: IDCompositionSaturationEffect::SetSaturation(float) (dcomp.h)
author: windows-sdk-content
description: Sets the saturation of the image.
old-location: directcomp\idcompositionsaturationeffect_setsaturation.htm
tech.root: directcomp
ms.assetid: A2BAE19A-FC9F-4476-9DBB-438FE2923246
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionSaturationEffect interface [DirectComposition],SetSaturation method, IDCompositionSaturationEffect.SetSaturation, IDCompositionSaturationEffect.SetSaturation(float), IDCompositionSaturationEffect::SetSaturation, IDCompositionSaturationEffect::SetSaturation(float), SetSaturation, SetSaturation method [DirectComposition], SetSaturation method [DirectComposition],IDCompositionSaturationEffect interface, dcomp/IDCompositionSaturationEffect::SetSaturation, directcomp.idcompositionsaturationeffect_setsaturation
ms.topic: method
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - IDCompositionSaturationEffect.SetSaturation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionSaturationEffect::SetSaturation(float)


## -description


Sets the saturation of the image.


## -parameters




### -param ratio [in]

Type: <b>float</b>

The saturation of the image. You can set the saturation to a value between 0 and 1. If you set it to 1 the output image is fully saturated.
            If you set it to 0 the output image is monochrome. The saturation value is unitless.
            
            The effect calculates a color matrix based on the saturation value (s in the equation here) using the following equation:
            

<img alt="Matrix equation" src="./images/saturation_formula.png"/>

## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/ADA7C54C-E237-4455-8808-962A631B37E0">IDCompositionSaturationEffect</a>
 

 

