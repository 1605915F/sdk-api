---
UID: NF:mspstrm.CMSPStream.GetState
title: CMSPStream::GetState (mspstrm.h)
author: windows-sdk-content
description: The GetState method is called by the MSPCall object. It returns the current status of the stream. The default implementation returns E_NOTIMPL.
old-location: tapi3\cmspstream_getstate.htm
tech.root: Tapi
ms.assetid: 03fc3801-8bd4-432a-b0ca-f6506bd8c788
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CMSPStream interface [TAPI 2.2],GetState method, CMSPStream.GetState, CMSPStream::GetState, GetState, GetState method [TAPI 2.2], GetState method [TAPI 2.2],CMSPStream interface, _tapi3_cmspstream_getstate, mspstrm/CMSPStream::GetState, tapi3.cmspstream_getstate
ms.topic: method
req.header: mspstrm.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mspstrm.h
api_name:
 - CMSPStream.GetState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# CMSPStream::GetState


## -description


The 
<b>GetState</b> method is called by the MSPCall object. It returns the current status of the stream. The default implementation returns E_NOTIMPL.


## -parameters




### -param pdwStatus

Pointer to indication of stream's state. The precise return value is implementation dependent. An example set of types that might be defined for this purpose: STRM_RUNNING, STRM_PAUSED, and STRM_STOPPED.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms726913(v=VS.85).aspx">CMSPStream</a>
 

 

