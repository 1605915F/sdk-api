---
UID: NF:wmsdkidl.IWMSyncReader.OpenStream
title: IWMSyncReader::OpenStream
author: windows-sdk-content
description: The OpenStream method opens a stream for reading.
old-location: wmformat\iwmsyncreader_openstream.htm
tech.root: wmformat
ms.assetid: ef42495a-2565-4925-882e-c3c42f9d418b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWMSyncReader interface [windows Media Format],OpenStream method, IWMSyncReader.OpenStream, IWMSyncReader::OpenStream, IWMSyncReaderOpenStream, OpenStream, OpenStream method [windows Media Format], OpenStream method [windows Media Format],IWMSyncReader interface, wmformat.iwmsyncreader_openstream, wmsdkidl/IWMSyncReader::OpenStream
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
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
 - IWMSyncReader.OpenStream
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWMSyncReader::OpenStream


## -description



The <b>OpenStream</b> method opens a stream for reading.




## -parameters




### -param pStream [in]

Pointer to an <b>IStream</b> interface.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/2a46e79f-084e-4173-ad0f-211d3065d81a">IWMSyncReader Interface</a>



<a href="https://msdn.microsoft.com/dab1a9c4-487c-4b20-909e-05f3504698f5">IWMSyncReader::Open</a>
 

 

