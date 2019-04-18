---
UID: NF:certenroll.IX509SCEPEnrollment.ProcessResponseMessage
title: IX509SCEPEnrollment::ProcessResponseMessage (certenroll.h)
author: windows-sdk-content
description: Process a response message and return the disposition of the message.
old-location: security\ix509scepenrollment_processresponsemessage.htm
tech.root: seccertenroll
ms.assetid: 4254fdf3-473f-4f22-a08f-13481fd9f779
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IX509SCEPEnrollment interface [Security],ProcessResponseMessage method, IX509SCEPEnrollment.ProcessResponseMessage, IX509SCEPEnrollment::ProcessResponseMessage, ProcessResponseMessage, ProcessResponseMessage method [Security], ProcessResponseMessage method [Security],IX509SCEPEnrollment interface, certenroll/IX509SCEPEnrollment::ProcessResponseMessage, security.ix509scepenrollment_processresponsemessage
ms.topic: method
req.header: certenroll.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certenroll.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Certenroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Certenroll.dll
api_name:
 - IX509SCEPEnrollment.ProcessResponseMessage
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IX509SCEPEnrollment::ProcessResponseMessage


## -description


Process a response message and return the disposition of the message.


## -parameters




### -param strResponse [in]


### -param Encoding [in]


### -param pDisposition [out, retval]


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



You must call the <a href="https://msdn.microsoft.com/dcb887ab-c8b7-42e7-8b49-93755d24ba70">Initialize</a> and <a href="https://msdn.microsoft.com/b86d6dc3-aa96-45f3-9551-f24c39ea6cbf">CreateRequestMessage</a> methods or the <a href="https://msdn.microsoft.com/6b6f9e9d-5316-4928-861a-22497e1f5c00">InitializeForPending</a> method before calling this method.




## -see-also




<a href="https://msdn.microsoft.com/fcbac911-9e37-4994-bbb6-544b19a92749">IX509SCEPEnrollment</a>
 

 

