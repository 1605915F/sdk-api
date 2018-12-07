---
UID: NF:mfmediaengine.IMFMediaEngineSupportsSourceTransfer.DetachMediaSource
title: IMFMediaEngineSupportsSourceTransfer::DetachMediaSource
author: windows-sdk-content
description: Detaches the media source.
old-location: mf\imfmediaenginesupportssourcetransfer_detachmediasource.htm
tech.root: medfound
ms.assetid: a085fc53-91a3-46bb-862c-dde16fb7fa42
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DetachMediaSource, DetachMediaSource method [Media Foundation], DetachMediaSource method [Media Foundation],IMFMediaEngineSupportsSourceTransfer interface, IMFMediaEngineSupportsSourceTransfer interface [Media Foundation],DetachMediaSource method, IMFMediaEngineSupportsSourceTransfer.DetachMediaSource, IMFMediaEngineSupportsSourceTransfer::DetachMediaSource, mf.imfmediaenginesupportssourcetransfer_detachmediasource, mfmediaengine/IMFMediaEngineSupportsSourceTransfer::DetachMediaSource
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mfmediaengine.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mfmediaengine.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfmediaengine.h
api_name:
 - IMFMediaEngineSupportsSourceTransfer.DetachMediaSource
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFMediaEngineSupportsSourceTransfer::DetachMediaSource


## -description


Detaches the media source.


## -parameters




### -param ppByteStream [out]

Receives the byte stream.


### -param ppMediaSource [out]

Receives the media source.


### -param ppMSE [out]

Receives the media source extension.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/8784dcc2-52f4-41d9-a0ae-3ea7a736b604">IMFMediaEngineSupportsSourceTransfer</a>
 

 

