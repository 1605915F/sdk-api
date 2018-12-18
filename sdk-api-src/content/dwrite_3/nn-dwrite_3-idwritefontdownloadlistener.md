---
UID: NN:dwrite_3.IDWriteFontDownloadListener
title: IDWriteFontDownloadListener
author: windows-sdk-content
description: Application-defined callback interface that receives notifications from the font download queue (IDWriteFontDownloadQueue interface).
old-location: directwrite\idwritefontdownloadlistener.htm
tech.root: DirectWrite
ms.assetid: 92678d34-9a14-8d58-129c-be31a0963942
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDWriteFontDownloadListener, IDWriteFontDownloadListener interface [Direct Write], IDWriteFontDownloadListener interface [Direct Write],described, directwrite.idwritefontdownloadlistener, dwrite_3/IDWriteFontDownloadListener
ms.topic: interface
req.header: dwrite_3.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dwrite.lib
req.dll: Dwrite.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dwrite.dll
api_name:
 - IDWriteFontDownloadListener
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontDownloadListener interface


## -description


 Application-defined callback interface that receives notifications from the font  download queue (<a href="https://msdn.microsoft.com/en-us/library/Dn890778(v=VS.85).aspx">IDWriteFontDownloadQueue</a> 
  interface). Callbacks will occur on the downloading thread, and objects must be prepared to handle calls on their methods from other threads at any time.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDWriteFontDownloadListener</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IDWriteFontDownloadListener</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDWriteFontDownloadListener</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn890776(v=VS.85).aspx">DownloadCompleted</a>
</td>
<td align="left" width="63%">
The DownloadCompleted method is called back on an arbitrary thread when a    
    download operation ends. 

</td>
</tr>
</table> 

