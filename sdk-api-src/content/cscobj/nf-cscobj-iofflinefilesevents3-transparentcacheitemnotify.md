---
UID: NF:cscobj.IOfflineFilesEvents3.TransparentCacheItemNotify
title: IOfflineFilesEvents3::TransparentCacheItemNotify (cscobj.h)
author: windows-sdk-content
description: Reports that an action has been performed on a transparently cached item.
old-location: of\iofflinefilesevents3_transparentcacheitemnotify.htm
tech.root: offlinefiles
ms.assetid: 59bd7a71-0189-4c4d-a737-e6a3f09a533d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IOfflineFilesEvents3 interface [Offline Files],TransparentCacheItemNotify method, IOfflineFilesEvents3.TransparentCacheItemNotify, IOfflineFilesEvents3::TransparentCacheItemNotify, TransparentCacheItemNotify, TransparentCacheItemNotify method [Offline Files], TransparentCacheItemNotify method [Offline Files],IOfflineFilesEvents3 interface, cscobj/IOfflineFilesEvents3::TransparentCacheItemNotify, of.iofflinefilesevents3_transparentcacheitemnotify
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
 - IOfflineFilesEvents3.TransparentCacheItemNotify
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IOfflineFilesEvents3::TransparentCacheItemNotify


## -description


Reports that an action has been performed on a transparently cached item.


## -parameters




### -param pszPath [in]

The item's UNC path string.


### -param EventType [in]

An <a href="https://msdn.microsoft.com/4ab65756-5985-4240-805d-2221db3d1459">OFFLINEFILES_EVENTS</a> enumeration value that indicates the type of the item.


### -param ItemType [in]

An <a href="https://msdn.microsoft.com/cf8bb079-d691-4b37-b408-d1af1746ed37">OFFLINEFILES_ITEM_TYPE</a> enumeration value that indicates the type of the item.


### -param bModifiedData [in]

<b>TRUE</b> if the item's data was modified, <b>FALSE</b> otherwise.


### -param bModifiedAttributes [in]

<b>TRUE</b> if one or more of the item's attributes were modified, <b>FALSE</b> otherwise.


### -param pzsOldPath [in]

The original UNC path string for the item.


## -returns



Returns <b>S_OK</b> if successful, or an error value otherwise.




## -see-also




<a href="https://msdn.microsoft.com/f68c2c0c-e4f7-4048-99c9-761f98928157">IOfflineFilesEvents3</a>



<a href="https://msdn.microsoft.com/7f8656e0-0f24-46a0-81b7-62067b0d4c21">IOfflineFilesTransparentCacheInfo::IsTransparentlyCached</a>
 

 

