---
UID: NF:mfcaptureengine.IMFCapturePreviewSink.SetSampleCallback
title: IMFCapturePreviewSink::SetSampleCallback (mfcaptureengine.h)
author: windows-sdk-content
description: Sets a callback to receive the preview data for one stream.
old-location: mf\imfcapturepreviewsink_setsamplecallback.htm
tech.root: medfound
ms.assetid: 0E14E3E4-25C7-4FCA-B220-20E346E66933
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMFCapturePreviewSink interface [Media Foundation],SetSampleCallback method, IMFCapturePreviewSink.SetSampleCallback, IMFCapturePreviewSink::SetSampleCallback, SetSampleCallback, SetSampleCallback method [Media Foundation], SetSampleCallback method [Media Foundation],IMFCapturePreviewSink interface, mf.imfcapturepreviewsink_setsamplecallback, mfcaptureengine/IMFCapturePreviewSink::SetSampleCallback
ms.topic: method
req.header: mfcaptureengine.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfcaptureengine.h
api_name:
 - IMFCapturePreviewSink.SetSampleCallback
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFCapturePreviewSink::SetSampleCallback


## -description


Sets a callback to receive the preview data for one stream.


## -parameters




### -param dwStreamSinkIndex [in]

The zero-based index of the stream. The index is returned in the <i>pdwSinkStreamIndex</i> parameter of the <a href="https://msdn.microsoft.com/5D7A1FE0-92B9-4CC4-A268-17FA848055A9">IMFCaptureSink::AddStream</a> method.


### -param pCallback [in]

A pointer to the <a href="https://msdn.microsoft.com/7C621525-CCD2-45EC-9E7A-3A774B96EA6F">IMFCaptureEngineOnSampleCallback</a> interface. The caller must implement this interface.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Calling this method overrides any previous call to <a href="https://msdn.microsoft.com/98D3EFC4-841D-41EC-BC5C-E67029663864">IMFCapturePreviewSink::SetRenderHandle</a>.




## -see-also




<a href="https://msdn.microsoft.com/5E64C24D-D6EC-419B-9DC8-309EBCE0077E">IMFCapturePreviewSink</a>
 

 

