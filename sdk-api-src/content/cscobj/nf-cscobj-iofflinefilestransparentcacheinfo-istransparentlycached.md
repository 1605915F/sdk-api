---
UID: NF:cscobj.IOfflineFilesTransparentCacheInfo.IsTransparentlyCached
title: IOfflineFilesTransparentCacheInfo::IsTransparentlyCached
author: windows-sdk-content
description: Determines whether the item is transparently cached.
old-location: of\iofflinefilestransparentcacheinfo_istransparentlycached.htm
tech.root: offlinefiles
ms.assetid: 7f8656e0-0f24-46a0-81b7-62067b0d4c21
ms.author: windowssdkdev
ms.date: 11/16/2018
ms.keywords: IOfflineFilesTransparentCacheInfo interface [Offline Files],IsTransparentlyCached method, IOfflineFilesTransparentCacheInfo.IsTransparentlyCached, IOfflineFilesTransparentCacheInfo::IsTransparentlyCached, IsTransparentlyCached, IsTransparentlyCached method [Offline Files], IsTransparentlyCached method [Offline Files],IOfflineFilesTransparentCacheInfo interface, cscobj/IOfflineFilesTransparentCacheInfo::IsTransparentlyCached, of.iofflinefilestransparentcacheinfo_istransparentlycached
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
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
 - IOfflineFilesTransparentCacheInfo.IsTransparentlyCached
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOfflineFilesTransparentCacheInfo::IsTransparentlyCached


## -description


Determines whether the item is transparently cached.


## -parameters




### -param pbTransparentlyCached [out]

A pointer to a variable that receives <b>TRUE</b> if the item is transparently cached, or <b>FALSE</b> otherwise.


## -returns



Returns <b>S_OK</b> if successful, or an error value otherwise.




## -remarks



A transparently cached item is cached locally. However, it can be accessed only when the server is available and the user is online with respect to that server. If the cached version of the file matches the currect version of the file on the server, requests to read data will be satisfied from the cache rather than requesting the data from the server.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd442648(v=VS.85).aspx">IOfflineFilesEvents3::TransparentCacheItemNotify</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd442650(v=VS.85).aspx">IOfflineFilesTransparentCacheInfo</a>
 

 

