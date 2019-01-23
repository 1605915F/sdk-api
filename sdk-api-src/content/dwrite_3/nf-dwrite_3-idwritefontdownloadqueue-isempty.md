---
UID: NF:dwrite_3.IDWriteFontDownloadQueue.IsEmpty
title: IDWriteFontDownloadQueue::IsEmpty
author: windows-sdk-content
description: Determines whether the download queue is empty. Note that the queue does not include requests that are already being downloaded. Calling BeginDownloadclears the queue.
old-location: directwrite\idwritefontdownloadqueue_isempty.htm
tech.root: DirectWrite
ms.assetid: 2f1f0d1c-0db8-c382-7879-92a889cfeb6b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDWriteFontDownloadQueue interface [Direct Write],IsEmpty method, IDWriteFontDownloadQueue.IsEmpty, IDWriteFontDownloadQueue::IsEmpty, IsEmpty, IsEmpty method [Direct Write], IsEmpty method [Direct Write],IDWriteFontDownloadQueue interface, directwrite.idwritefontdownloadqueue_isempty, dwrite_3/IDWriteFontDownloadQueue::IsEmpty
ms.topic: method
req.header: dwrite_3.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
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
 - IDWriteFontDownloadQueue.IsEmpty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontDownloadQueue::IsEmpty


## -description


Determines whether the download queue is empty. Note that the queue does not    
    include requests that are already being downloaded. Calling <a href="https://msdn.microsoft.com/1e3b200c-0190-f600-1cb6-4e2a46f882b4">BeginDownload</a>clears the queue.


## -parameters






## -returns



Type: <b>BOOL</b>

TRUE if the queue is empty, FALSE if there are requests pending for <a href="https://msdn.microsoft.com/1e3b200c-0190-f600-1cb6-4e2a46f882b4">BeginDownload</a>.




## -see-also




<a href="https://msdn.microsoft.com/d1b1dfab-a22a-40bb-ffc4-eb094ac14217">IDWriteFontDownloadQueue</a>
 

 

