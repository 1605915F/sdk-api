---
UID: NF:mspcall.CMSPCallMultiGraph.InternalCreateStream
title: CMSPCallMultiGraph::InternalCreateStream (mspcall.h)
author: windows-sdk-content
description: The InternalCreateStream method is called by CreateStream to create a stream object (the caller does the argument checking).
old-location: tapi3\cmspcallmultigraph_internalcreatestream.htm
tech.root: Tapi
ms.assetid: 62d098d5-b9cd-4e64-bec8-c4f736be22f9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: CMSPCallMultiGraph interface [TAPI 2.2],InternalCreateStream method, CMSPCallMultiGraph.InternalCreateStream, CMSPCallMultiGraph::InternalCreateStream, InternalCreateStream, InternalCreateStream method [TAPI 2.2], InternalCreateStream method [TAPI 2.2],CMSPCallMultiGraph interface, _tapi3_cmspcallmultigraph_internalcreatestream, mspcall/CMSPCallMultiGraph::InternalCreateStream, tapi3.cmspcallmultigraph_internalcreatestream
ms.topic: method
req.header: mspcall.h
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
 - Mspcall.h
api_name:
 - CMSPCallMultiGraph.InternalCreateStream
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CMSPCallMultiGraph::InternalCreateStream


## -description


The 
<b>InternalCreateStream</b> method is called by 
<a href="https://msdn.microsoft.com/402cde43-6b2a-4e4e-bf46-97fcafb7574a">CreateStream</a> to create a stream object (the caller does the argument checking). It creates and initializes the stream object (using 
<a href="https://msdn.microsoft.com/en-us/library/ms726500(v=VS.85).aspx">CreateStreamObject</a>). It uses <b>CoCreateInstance</b> to create a filter graph for the stream. It calls 
<a href="https://msdn.microsoft.com/en-us/library/ms726610(v=VS.85).aspx">RegisterWaitEvent</a> to start waiting for events on the filter graph. It adds the stream into the call object's list of stream objects. It addrefs the stream pointer and returns it.


## -parameters




### -param dwMediaType

Descriptor of 
<a href="https://msdn.microsoft.com/3e418c9a-a008-4b94-b5d2-7c2eccb3bf87">media type</a> for stream.


### -param Direction

Descriptor of 
<a href="https://msdn.microsoft.com/55ef9df3-1b85-439b-8ecb-28e5069390b9">terminal direction</a>.


### -param ppStream

Pointer to array of 
<a href="https://msdn.microsoft.com/74a385c8-0c36-4cf0-8983-5ffd7b0e5c4a">ITStream</a> interfaces.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms726558(v=VS.85).aspx">CMSPCallMultiGraph</a>
 

 

