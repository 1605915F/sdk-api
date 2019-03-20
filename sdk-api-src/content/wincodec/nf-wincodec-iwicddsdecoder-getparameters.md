---
UID: NF:wincodec.IWICDdsDecoder.GetParameters
title: IWICDdsDecoder::GetParameters (wincodec.h)
author: windows-sdk-content
description: Gets DDS-specific data.
old-location: wic\iwicddsdecoder_getparameters.htm
tech.root: wic
ms.assetid: D4EE39D6-54DC-450D-A430-2996D349BEC6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetParameters, GetParameters method [Windows Imaging Component], GetParameters method [Windows Imaging Component],IWICDdsDecoder interface, IWICDdsDecoder interface [Windows Imaging Component],GetParameters method, IWICDdsDecoder.GetParameters, IWICDdsDecoder::GetParameters, wic.iwicddsdecoder_getparameters, wincodec/IWICDdsDecoder::GetParameters
ms.topic: method
req.header: wincodec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wincodec.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Windowscodecs.lib
req.dll: Windowscodecs.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Windowscodecs.dll
api_name:
 - IWICDdsDecoder.GetParameters
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWICDdsDecoder::GetParameters


## -description


Gets DDS-specific data.


## -parameters




### -param pParameters [out]

Type: <b><a href="https://msdn.microsoft.com/2E5755B4-E8DC-40B2-8DA1-B053A261079B">WICDdsParameters</a>*</b>

A pointer to the structure where the information is returned.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/632D1E7B-9C1D-48FB-95B5-1A295FE99577">IWICDdsDecoder</a>



<a href="https://msdn.microsoft.com/2E5755B4-E8DC-40B2-8DA1-B053A261079B">WICDdsParameters</a>
 

 

