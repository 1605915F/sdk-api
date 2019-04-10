---
UID: NF:mfidl.IMFHttpDownloadRequest.EndSendRequest
title: IMFHttpDownloadRequest::EndSendRequest (mfidl.h)
author: windows-sdk-content
description: Invoked by Microsoft Media Foundation to complete the asynchronous operation started by BeginSendRequest.
old-location: mf\imfhttpdownloadrequest_endsendrequest.htm
tech.root: medfound
ms.assetid: 2B1554C7-2814-4A9E-BBAC-B25C78775420
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: EndSendRequest, EndSendRequest method [Media Foundation], EndSendRequest method [Media Foundation],IMFHttpDownloadRequest interface, IMFHttpDownloadRequest interface [Media Foundation],EndSendRequest method, IMFHttpDownloadRequest.EndSendRequest, IMFHttpDownloadRequest::EndSendRequest, mf.imfhttpdownloadrequest_endsendrequest, mfidl/IMFHttpDownloadRequest::EndSendRequest
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1703 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfplat.lib; Mfplat.dll
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - mfplat.lib
 - mfplat.dll
 - mfplat.dll
 - mfplat.dll.dll
api_name:
 - IMFHttpDownloadRequest.EndSendRequest
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMFHttpDownloadRequest::EndSendRequest


## -description


Invoked by Microsoft Media Foundation to complete the asynchronous operation started by <a href="https://msdn.microsoft.com/38025B19-146A-4050-9BD2-2CF974729FE3">BeginSendRequest</a>.


## -parameters




### -param pResult [in]

Pointer to the <a href="https://msdn.microsoft.com/8c95b1de-8974-445c-8070-41552ea83e53">IMFAsyncResult</a> interface. Microsoft Media Foundation will pass in the same pointer that its callback object received in the <a href="https://msdn.microsoft.com/22473605-637e-4783-a8cb-98248b0a0327">IMFAsyncCallback::Invoke</a> method.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.
          

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The request was successfully sent to the server.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/A8A37C2F-A662-4FDA-95F6-43D96A8471A8">IMFHttpDownloadRequest</a>
 

 

