---
UID: NF:dcomp.IDCompositionLinearTransferEffect.SetAlphaYIntercept(IDCompositionAnimation)
title: IDCompositionLinearTransferEffect::SetAlphaYIntercept(IDCompositionAnimation)
author: windows-sdk-content
description: Sets the Y-intercept of the linear function for the Alpha channel.
old-location: directcomp\idcompositionlineartransfereffect_setalphayintercept_2.htm
tech.root: directcomp
ms.assetid: 805D778A-DDB2-4BF6-9029-65A55C1F490F
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionLinearTransferEffect interface [DirectComposition],SetAlphaYIntercept method, IDCompositionLinearTransferEffect.SetAlphaYIntercept, IDCompositionLinearTransferEffect.SetAlphaYIntercept(IDCompositionAnimation), IDCompositionLinearTransferEffect::SetAlphaYIntercept, IDCompositionLinearTransferEffect::SetAlphaYIntercept(IDCompositionAnimation), SetAlphaYIntercept, SetAlphaYIntercept method [DirectComposition], SetAlphaYIntercept method [DirectComposition],IDCompositionLinearTransferEffect interface, dcomp/IDCompositionLinearTransferEffect::SetAlphaYIntercept, directcomp.idcompositionlineartransfereffect_setalphayintercept_2
ms.prod: windows-hardware
ms.technology: windows-devices
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
 - IDCompositionLinearTransferEffect.SetAlphaYIntercept
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionLinearTransferEffect::SetAlphaYIntercept(IDCompositionAnimation)


## -description


Sets the Y-intercept of the linear function for the Alpha channel.


## -parameters




### -param animation [in]

Type: <b><a href="https://msdn.microsoft.com/f914e14b-4ac0-4591-9b7f-6b45b88baaaa">IDCompositionAnimation</a>*</b>

An animation that represents how the the Y-intercept of the linear function for the alpha channel. changes over time. This parameter must not be NULL.


## -returns



Type: <b><a href="455d07e9-52c3-4efb-a9dc-2955cbfd38cc">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/516CD029-DBB1-4AD7-92BB-8B6EF6C733FA">IDCompositionLinearTransferEffect</a>
 

 

