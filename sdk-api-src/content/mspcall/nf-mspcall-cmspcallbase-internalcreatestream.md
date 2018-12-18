---
UID: NF:mspcall.CMSPCallBase.InternalCreateStream
title: CMSPCallBase::InternalCreateStream
author: windows-sdk-content
description: The InternalCreateStream method is called by CreateStream to create a stream object (the caller does the argument checking). It should create and initialize the stream object (using CreateStreamObject).
old-location: tapi3\cmspcallbase_internalcreatestream.htm
tech.root: tapi
ms.assetid: 6f9cef2e-36dd-4095-9060-b6d37ccbc6d7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CMSPCallBase interface [TAPI 2.2],InternalCreateStream method, CMSPCallBase.InternalCreateStream, CMSPCallBase::InternalCreateStream, InternalCreateStream, InternalCreateStream method [TAPI 2.2], InternalCreateStream method [TAPI 2.2],CMSPCallBase interface, _tapi3_cmspcallbase_internalcreatestream, mspcall/CMSPCallBase::InternalCreateStream, tapi3.cmspcallbase_internalcreatestream
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
 - CMSPCallBase.InternalCreateStream
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CMSPCallBase::InternalCreateStream


## -description


The 
<b>InternalCreateStream</b> method is called by 
<a href="https://msdn.microsoft.com/402cde43-6b2a-4e4e-bf46-97fcafb7574a">CreateStream</a> to create a stream object (the caller does the argument checking). It should create and initialize the stream object (using 
<a href="https://msdn.microsoft.com/en-us/library/ms726500(v=VS.85).aspx">CreateStreamObject</a>).


## -parameters




### -param dwMediaType


<a href="https://msdn.microsoft.com/3e418c9a-a008-4b94-b5d2-7c2eccb3bf87">Media type</a> or types of call.


### -param Direction

Indicates 
<a href="https://msdn.microsoft.com/55ef9df3-1b85-439b-8ecb-28e5069390b9">terminal direction</a>.


### -param ppStream

Pointer to 
<a href="https://msdn.microsoft.com/74a385c8-0c36-4cf0-8983-5ffd7b0e5c4a">ITStream</a> object interface.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms726496(v=VS.85).aspx">CMSPCallBase</a>



<a href="https://msdn.microsoft.com/en-us/library/ms726578(v=VS.85).aspx">CMSPCallMultiGraph::InternalCreateStream</a>



<a href="https://msdn.microsoft.com/402cde43-6b2a-4e4e-bf46-97fcafb7574a">CreateStream</a>



<a href="https://msdn.microsoft.com/en-us/library/ms726500(v=VS.85).aspx">CreateStreamObject</a>



<a href="https://msdn.microsoft.com/74a385c8-0c36-4cf0-8983-5ffd7b0e5c4a">ITStream</a>
 

 

