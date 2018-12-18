---
UID: NF:cscobj.IOfflineFilesChangeInfo.IsLocallyModifiedTime
title: IOfflineFilesChangeInfo::IsLocallyModifiedTime
author: windows-sdk-content
description: Determines whether one or more of an item's time values were modified while working offline.
old-location: of\iofflinefileschangeinfo_islocallymodifiedtime.htm
tech.root: offlinefiles
ms.assetid: 7b88bf6d-f5a7-48e3-8c0a-41a8f6fba91f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOfflineFilesChangeInfo interface [Offline Files],IsLocallyModifiedTime method, IOfflineFilesChangeInfo.IsLocallyModifiedTime, IOfflineFilesChangeInfo::IsLocallyModifiedTime, IsLocallyModifiedTime, IsLocallyModifiedTime method [Offline Files], IsLocallyModifiedTime method [Offline Files],IOfflineFilesChangeInfo interface, cscobj/IOfflineFilesChangeInfo::IsLocallyModifiedTime, of.iofflinefileschangeinfo_islocallymodifiedtime
ms.topic: method
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: CscSvc.dll; CscObj.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - CscSvc.dll
 - CscObj.dll
api_name:
 - IOfflineFilesChangeInfo.IsLocallyModifiedTime
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOfflineFilesChangeInfo::IsLocallyModifiedTime


## -description


Determines whether one or more of an item's time values were modified while working offline.


## -parameters




### -param pbLocallyModifiedTime [out]

Receives <b>TRUE</b> if one or more of the item's time values were modified in the Offline Files cache while working offline, or <b>FALSE</b> otherwise.


## -returns



Returns <b>S_OK</b> if successful, or an error value otherwise.




## -remarks



Use <a href="https://msdn.microsoft.com/120b3f7c-6a92-4a03-8676-1ad4e4dc96b3">IOfflineFilesFileSysInfo::GetTimes</a> to examine the time values associated with an item.




## -see-also




<a href="https://msdn.microsoft.com/0ece6120-bd5d-4e3d-b71f-7aa9a51a1568">IOfflineFilesChangeInfo</a>
 

 

