---
UID: NF:cscobj.IOfflineFilesEvents.ItemDeletedFromCache
title: IOfflineFilesEvents::ItemDeletedFromCache (cscobj.h)
author: windows-sdk-content
description: Reports that an item has been removed from the Offline Files cache.
old-location: of\iofflinefilesevents_itemdeletedfromcache.htm
tech.root: offlinefiles
ms.assetid: 358b358a-65cc-4f37-8beb-be492b83c222
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IOfflineFilesEvents interface [Offline Files],ItemDeletedFromCache method, IOfflineFilesEvents.ItemDeletedFromCache, IOfflineFilesEvents::ItemDeletedFromCache, ItemDeletedFromCache, ItemDeletedFromCache method [Offline Files], ItemDeletedFromCache method [Offline Files],IOfflineFilesEvents interface, cscobj/IOfflineFilesEvents::ItemDeletedFromCache, of.iofflinefilesevents_itemdeletedfromcache
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
 - IOfflineFilesEvents.ItemDeletedFromCache
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOfflineFilesEvents::ItemDeletedFromCache


## -description


Reports that an item has been removed from the Offline Files cache.


## -parameters




### -param pszPath [in]

The item's UNC path string.


### -param ItemType [in]

An <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/cscobj/ne-cscobj-tagofflinefiles_item_type">OFFLINEFILES_ITEM_TYPE</a> enumeration value that indicates the type of the item.


## -returns



The return value is ignored.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/cscobj/nn-cscobj-iofflinefilesevents">IOfflineFilesEvents</a>
 

 

