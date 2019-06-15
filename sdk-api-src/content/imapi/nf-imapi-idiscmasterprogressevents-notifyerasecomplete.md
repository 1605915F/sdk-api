---
UID: NF:imapi.IDiscMasterProgressEvents.NotifyEraseComplete
title: IDiscMasterProgressEvents::NotifyEraseComplete (imapi.h)
author: windows-sdk-content
description: Notifies an application that a call to IDiscRecorder::Erase has finished.
old-location: imapi\idiscmasterprogressevents_notifyerasecomplete.htm
tech.root: imapi
ms.assetid: 17a0debe-919d-4db7-bcbb-eb4fc9973d83
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IDiscMasterProgressEvents interface [IMAPI],NotifyEraseComplete method, IDiscMasterProgressEvents.NotifyEraseComplete, IDiscMasterProgressEvents::NotifyEraseComplete, NotifyEraseComplete, NotifyEraseComplete method [IMAPI], NotifyEraseComplete method [IMAPI],IDiscMasterProgressEvents interface, _win32_idiscmasterprogressevents_notifyerasecomplete, base.idiscmasterprogressevents_notifyerasecomplete, imapi.idiscmasterprogressevents_notifyerasecomplete, imapi/IDiscMasterProgressEvents::NotifyEraseComplete
ms.topic: method
req.header: imapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Uuid.lib
req.dll: Actxprxy.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Actxprxy.dll
api_name:
 - IDiscMasterProgressEvents.NotifyEraseComplete
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDiscMasterProgressEvents::NotifyEraseComplete


## -description


Notifies an application that a call to 
<a href="https://docs.microsoft.com/windows/desktop/api/imapi/nf-imapi-idiscrecorder-erase">IDiscRecorder::Erase</a> has finished.


## -parameters




### -param status [in]

Status code to be returned from 
<a href="https://docs.microsoft.com/windows/desktop/api/imapi/nf-imapi-idiscrecorder-erase">IDiscRecorder::Erase</a>.


## -returns



S_OK is returned on success, but other success codes may be returned as a result of implementation. The following error codes are commonly returned on operation failure, but do not represent the only possible error values:




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/imapi/nn-imapi-idiscmasterprogressevents">IDiscMasterProgressEvents</a>
 

 

