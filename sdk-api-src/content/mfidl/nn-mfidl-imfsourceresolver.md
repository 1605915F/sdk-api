---
UID: NN:mfidl.IMFSourceResolver
title: IMFSourceResolver (mfidl.h)
author: windows-sdk-content
description: Creates a media source from a URL or a byte stream.
old-location: mf\imfsourceresolver.htm
tech.root: medfound
ms.assetid: 079c61c5-7a29-4411-840e-9349190726ac
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: 079c61c5-7a29-4411-840e-9349190726ac, IMFSourceResolver, IMFSourceResolver interface [Media Foundation], IMFSourceResolver interface [Media Foundation],described, mf.imfsourceresolver, mfidl/IMFSourceResolver
ms.topic: interface
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfuuid.lib
 - mfuuid.dll
api_name:
 - IMFSourceResolver
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFSourceResolver interface


## -description


Creates a media source from a URL or a byte stream. The <a href="https://msdn.microsoft.com/93eecf10-308b-4bb4-92f9-fd32d6ecdb04">Source Resolver</a> implements this interface. To create the source resolver, call <a href="https://msdn.microsoft.com/60d6b0e2-5ab2-4a20-99d9-e6b806a1f576">MFCreateSourceResolver</a> function.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMFSourceResolver</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IMFSourceResolver</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMFSourceResolver</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6e218b93-4855-40dd-96cc-c4ee02792c14">BeginCreateObjectFromByteStream</a>
</td>
<td align="left" width="63%">
Begins an asynchronous request to create a media source from a byte stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/bc97c1fb-d23a-4887-b6ac-0751c254a405">BeginCreateObjectFromURL</a>
</td>
<td align="left" width="63%">
Begins an asynchronous request to create a media source or a byte stream from a URL.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/6a30ac92-a281-4293-8975-987fa25a5318">CancelObjectCreation</a>
</td>
<td align="left" width="63%">
Cancels an asynchronous request to create an object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/e4a4aad5-0924-4251-b0da-6919ae010bf0">CreateObjectFromByteStream</a>
</td>
<td align="left" width="63%">
Creates a media source from a byte stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b8f751b1-6456-4d67-839d-ecfa388e8d71">CreateObjectFromURL</a>
</td>
<td align="left" width="63%">
Creates a media source or a byte stream from a URL.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/54532c0e-772b-45b6-95a3-5959023b9bc8">EndCreateObjectFromByteStream</a>
</td>
<td align="left" width="63%">
Completes an asynchronous request to create a media source from a byte stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/af50a76d-b083-4815-bbff-820b21ff8d1b">EndCreateObjectFromURL</a>
</td>
<td align="left" width="63%">
Completes an asynchronous request to create an object from a URL.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/3e367190-4c88-430e-adbf-9837e1bf0d2b">Media Foundation Interfaces</a>



<a href="https://msdn.microsoft.com/93eecf10-308b-4bb4-92f9-fd32d6ecdb04">Source Resolver</a>
 

 

