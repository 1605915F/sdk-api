---
UID: NF:winml.IWinMLEvaluationContext.BindValue
title: IWinMLEvaluationContext::BindValue (winml.h)
author: windows-sdk-content
description: Binds the input/output to the given model.
old-location: machinelearning\iwinmlevaluationcontext_bindvalue_.htm
tech.root: MachineLearning
ms.assetid: 3D417952-92DD-4111-9060-C7F8CCA456AB
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: BindValue, BindValue method, BindValue method,IWinMLEvaluationContext interface, IWinMLEvaluationContext interface,BindValue method, IWinMLEvaluationContext.BindValue, IWinMLEvaluationContext::BindValue, MachineLearning.iwinmlevaluationcontext_bindvalue_, winml/IWinMLEvaluationContext::BindValue
ms.topic: method
req.header: winml.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1803 [desktop apps only]
req.target-min-winversvr: Windows Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Winml.lib
req.dll: Winml.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - winml.dll
api_name:
 - IWinMLEvaluationContext.BindValue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWinMLEvaluationContext::BindValue


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

<b>These APIs have been deprecated and should no longer be used:  </b>Please use <a href="https://docs.microsoft.com/uwp/api/windows.ai.machinelearning">Windows.AI.MachineLearning</a> instead.

Binds the input/output to the given model.


## -parameters




### -param pDescriptor [in]

A pointer to a <a href="https://msdn.microsoft.com/928C2AD0-73DD-4ECA-AC54-36ED84A9E4E6">WINML_BINDING_DESC</a> containing the input/output binding descriptor.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/D4C9B16A-B351-41E4-AD42-20C25F3CC404">IWinMLEvaluationContext</a>
 

 

