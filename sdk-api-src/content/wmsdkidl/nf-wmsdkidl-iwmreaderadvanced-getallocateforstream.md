---
UID: NF:wmsdkidl.IWMReaderAdvanced.GetAllocateForStream
title: IWMReaderAdvanced::GetAllocateForStream
author: windows-sdk-content
description: The GetAllocateForStream method ascertains whether the reader is configured to use IWMReaderCallbackAdvanced to allocate stream samples delivered by the IWMReaderCallbackAdvanced::OnStreamSample callback.
old-location: wmformat\iwmreaderadvanced_getallocateforstream.htm
tech.root: wmformat
ms.assetid: 816f13b1-9856-482d-b5b1-4aaf5c61c230
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAllocateForStream, GetAllocateForStream method [windows Media Format], GetAllocateForStream method [windows Media Format],IWMReaderAdvanced interface, IWMReaderAdvanced interface [windows Media Format],GetAllocateForStream method, IWMReaderAdvanced.GetAllocateForStream, IWMReaderAdvanced::GetAllocateForStream, IWMReaderAdvancedGetAllocateForStream, wmformat.iwmreaderadvanced_getallocateforstream, wmsdkidl/IWMReaderAdvanced::GetAllocateForStream
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 7 SDK, or later versions of the SDK
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
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wmvcore.lib
 - Wmvcore.dll
 - WMStubDRM.lib
 - WMStubDRM.dll
api_name:
 - IWMReaderAdvanced.GetAllocateForStream
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMReaderAdvanced::GetAllocateForStream


## -description



The <b>GetAllocateForStream</b> method ascertains whether the reader is configured to use <a href="https://msdn.microsoft.com/9d18961a-5ea4-4f3e-b473-7399e155f800">IWMReaderCallbackAdvanced</a> to allocate stream samples delivered by the <a href="https://msdn.microsoft.com/6bfdd903-a3a4-4ef4-b88a-4d24c9c0f4b8">IWMReaderCallbackAdvanced::OnStreamSample</a> callback.




## -parameters




### -param dwSreamNum [in]

<b>WORD</b> containing the stream number.


### -param pfAllocate [out]

Pointer to a Boolean value that is set to True if the reader uses <b>IWMReaderCallbackAdvanced</b> to allocate samples.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -remarks



Stream numbers are in the range of 1 through 63.




## -see-also




<a href="https://msdn.microsoft.com/a7a20f87-6f21-4fe8-8889-1b6689daf833">IWMReaderAdvanced Interface</a>



<a href="https://msdn.microsoft.com/58c396a9-5d1e-4a13-a877-5289649a6375">IWMReaderAdvanced::SetAllocateForStream</a>
 

 

