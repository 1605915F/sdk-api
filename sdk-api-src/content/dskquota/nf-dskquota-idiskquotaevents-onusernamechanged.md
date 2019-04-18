---
UID: NF:dskquota.IDiskQuotaEvents.OnUserNameChanged
title: IDiskQuotaEvents::OnUserNameChanged (dskquota.h)
author: windows-sdk-content
description: Notifies the client's connection sink whenever a user's SID has been asynchronously resolved.
old-location: fs\idiskquotaevents_onusernamechanged.htm
tech.root: FileIO
ms.assetid: d01cb679-03e2-4b76-b068-f64e576709fb
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IDiskQuotaEvents interface [Files],OnUserNameChanged method, IDiskQuotaEvents.OnUserNameChanged, IDiskQuotaEvents::OnUserNameChanged, OnUserNameChanged, OnUserNameChanged method [Files], OnUserNameChanged method [Files],IDiskQuotaEvents interface, _win32_idiskquotaevents_onusernamechanged, base.idiskquotaevents_onusernamechanged, dskquota/IDiskQuotaEvents::OnUserNameChanged, fs.idiskquotaevents_onusernamechanged
ms.topic: method
req.header: dskquota.h
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
req.lib: 
req.dll: Dskquota.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dskquota.dll
api_name:
 - IDiskQuotaEvents.OnUserNameChanged
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDiskQuotaEvents::OnUserNameChanged


## -description


Notifies the client's connection sink whenever a user's SID has been asynchronously resolved. If 
<a href="https://msdn.microsoft.com/d4027660-beb1-45eb-9dd3-f4c12df28051">IDiskQuotaUser::GetAccountStatus</a> returns DISKQUOTA_USER_ACCOUNT_RESOLVED, the user's account container name, logon name, and display name strings are available in the quota user object. 


## -parameters




### -param pUser [in]

A pointer to the 
<a href="https://msdn.microsoft.com/27edbebc-35b4-4f6a-87cc-d8a99782f405">IDiskQuotaUser</a> interface for the quota user object. Do not  call <a href="https://msdn.microsoft.com/en-us/library/ms682317(v=VS.85).aspx">Release</a> on this pointer. The <b>DiskQuotaControl</b> object controls the lifetime of the user object.


## -returns



The return value is ignored.




## -see-also




<a href="https://msdn.microsoft.com/c1f79e2e-834b-41dc-a15f-6dd1034d021b">Disk Management Interfaces</a>



<a href="https://msdn.microsoft.com/42efbd5b-6455-4319-a76e-cdb666fc36b8">Disk Quotas</a>



<a href="https://msdn.microsoft.com/4b5dcb1f-8edb-4fcb-94ea-2a627667071e">IDiskQuotaEvents</a>
 

 

