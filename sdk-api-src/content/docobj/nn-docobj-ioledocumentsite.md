---
UID: NN:docobj.IOleDocumentSite
title: IOleDocumentSite (docobj.h)
author: windows-sdk-content
description: Enables a document that has been implemented as a document object to bypass the normal activation sequence for in-place-active objects and to directly instruct its client site to activate it as a document object.
old-location: com\ioledocumentsite.htm
tech.root: com
ms.assetid: cac435c9-caee-4751-9ad8-df48b6d4c7e0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOleDocumentSite, IOleDocumentSite interface [COM], IOleDocumentSite interface [COM],described, _ole_ioledocumentsite, com.ioledocumentsite, docobj/IOleDocumentSite
ms.topic: interface
req.header: docobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: DocObj.Idl
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
 - DocObj.h
api_name:
 - IOleDocumentSite
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOleDocumentSite interface


## -description


Enables a document that has been implemented as a document object to bypass the normal activation sequence for in-place-active objects and to directly instruct its client site to activate it as a document object. A client site with this ability is called a document site.

For each document object to be hosted, a container must provide a corresponding document site, which is an OLE Documents client site that, in addition to implementing <a href="https://msdn.microsoft.com/dafee149-926a-4d08-a43d-5847682db645">IOleClientSite</a> and <a href="https://msdn.microsoft.com/bc9f217a-75bd-4155-9d00-df44b00cf0e5">IAdviseSink</a>, also implements <b>IOleDocumentSite</b>. Each document site implements a separate document view site object for each view of a document to be activated. The document view site implements <a href="https://msdn.microsoft.com/6d37e022-8c19-48b3-affb-e0eca19b5e05">IOleInPlaceSite</a> and, optionally, <a href="https://msdn.microsoft.com/55c960be-48e3-42e1-b459-49227be62171">IContinueCallback</a>.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IOleDocumentSite</b> interface inherits from the <a href="https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx">IUnknown</a> interface. <b>IOleDocumentSite</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IOleDocumentSite</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4e4a746d-460a-478e-9ca5-be5f63b03d17">ActivateMe</a>
</td>
<td align="left" width="63%">
Asks a document site to activate the document.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/dafee149-926a-4d08-a43d-5847682db645">IOleClientSite</a>



<a href="https://msdn.microsoft.com/8b022f2c-d4b4-44ca-8e69-46e9aa20b3f9">IOleControlSite</a>



<a href="https://msdn.microsoft.com/6d37e022-8c19-48b3-affb-e0eca19b5e05">IOleInPlaceSite</a>
 

 

